## How to install
You can find the scripts in the resource browser of the following .vwx file:
[ImportElevationExample.zip](files/ImportEvelationExample.zip)

## How the sample works
First you need to export longitude and latitude information of the selected objects into a .csv file using the first script in resource browser (ExportLongitudeLatitude).
Remember that for exporting you need to manually select the objects that you want before running the script:

```python
import vs
import os
import webbrowser
from tkinter import Tk

def execute():	
	vs.AlrtDialog( 'This script will export the selected 3D locuses in all layers into separate file to be used in the www.esurveyearth.com tool. Specify export file in the next dialog.' )
	file_path = vs.PutFile('Select the file to create:', 'New File.txt')
	
	numofSelectedObjects = 0
	if not vs.DidCancel():
		vs.Close(file_path)
		clipboard_copier = Tk()
		clipboard_copier.withdraw()
		clipboard_copier.clipboard_clear()
		clipboard_copier.clipboard_append(file_path)
		clipboard_copier.destroy()
		vs.AlrtDialog( 'File path :' +file_path + '\nhas been copied to clipboard. You can paste it anywhere with Ctrl+V or right click then paste')
		
		with open(file_path,'w') as fileHandle:
			hLayer = vs.GetParent( vs.FObject() )
			while hLayer != None:
				h = vs.FInLayer( hLayer );
				while h != None:
					if(vs.Selected(h)):						
						if(vs.GetTypeN(h) == 9):
							numofSelectedObjects += 1	
							currPoint = vs.GetLocus3D(h)
							isValid, outLat, outLon = vs.VWCoordToGeog(currPoint[0], currPoint[1])
							fileHandle.write(repr(outLat)+', '+repr(outLon)+'\n')	
							#fileHandle.write("{:.5f}".format(currPoint[0])+', '+"{:.5f}".format(currPoint[1])+'\n')							
						elif(vs.GetTypeN(h) == 5 or vs.GetTypeN(h) == 21):							
							numofSelectedObjects += 1
							numofVertices = vs.GetVertNum(h)
							for vertInd in range(1, numofVertices+1):														
								vertX, vertY = vs.GetPolyPt(h, vertInd)
								isValid, outLat, outLon = vs.VWCoordToGeog(vertX, vertY)
								fileHandle.write(repr(outLat)+', '+repr(outLon)+'\n')	
								
					h = vs.NextObj( h );
				hLayer = vs.NextLayer( hLayer );
			
			
			if(numofSelectedObjects > 0):
				vs.AlrtDialog( 'Now you are being redirected to surveyearth website to upload saved coordinates and get the elevations in .kml file' )
				url = 'http://www.esurveyearth.com/Index.aspx'
				# Open URL in a new tab, if a browser window is already open.
				webbrowser.open_new_tab(url)
			else:
				vs.AlrtDialog( 'No point was selected!\nPlease manually select points that you want to retrieve the elevation' )
			return

execute()
```

If execution is successful you will be redirected to the Survey Earth website. There you can upload the CSV file and get a .kml file which includes elevation information for each (Longitude, Latitude)

Now you can run the second script which would parse this kml file and import the elevation to those selected objects:

```python
import vs
import xml.etree.ElementTree as ET
import fileinput
import sys
import itertools, collections

def execute():
	vs.AlrtDialog('This script will load .kml file and will update elevation (z coordinate) of corresponding points in all layers')
	# file_path = vs.PutFile('Select the kml file:', '')
	is_file_selected, file_path = vs.GetFileN('Select the kml file:', '', 'kml')
	
	list_of_processedObjects = []
	
	if is_file_selected:
		with open(file_path) as input_file:
			
			input_file.seek(0) 
			first_chars = input_file.read(4)
			input_file.seek(0) 
			if first_chars != '<kml':
				vs.AlrtDialog('File with wrong format provided!')	
					
		for curr_line in fileinput.input(file_path, inplace=True):
			if(fileinput.isfirstline()):
				sys.stdout.write("<kml>\n")
			else:
				sys.stdout.write(curr_line)

		tree = ET.parse(file_path)
		root = tree.getroot()
		
		numofSelectedPoints = 0
		for child in  root.iter('Document'):
			pointIterator = child.iter('Placemark')
			for currPoint in pointIterator:
				for currXYPoint in currPoint.iter('Point'):
					txtLonCoordinate, txtLatCoordinate, alaki = currXYPoint.find('coordinates').text.strip().split(',')
					txtZCoordinate = float(currPoint.find('name').text)
					
					isValid, tempo = vs.GeogCoordToVW(float(txtLatCoordinate), float(txtLonCoordinate))
					txtXCoordinate = tempo[0]
					txtYCoordinate = tempo[1]
					#vs.AlrtDialog(str(txtXCoordinate))
										
					addPoint = False
					hLayer = vs.GetParent(vs.FObject())
					
					while hLayer != None:
	 					h = vs.FInLayer(hLayer);
	 					while h != None:
	 						if(h not in list_of_processedObjects):
		 						if(vs.GetTypeN(h) == 9):
		 							currVWPoint = vs.GetLocus3D(h)
		 							if("{:.6f}".format(currVWPoint[0]) == "{:.6f}".format(txtXCoordinate) and "{:.6f}".format(currVWPoint[1]) == "{:.6f}".format(txtYCoordinate)):
		 								vs.DelObject(h)
		 								vs.Locus3D(txtXCoordinate, txtYCoordinate, txtZCoordinate)
		 								list_of_processedObjects.append(vs.LNewObj())
					 					numofSelectedPoints += 1	 										 							 								
		 								break
	 							elif(vs.GetTypeN(h) == 5 or vs.GetTypeN(h) == 21):	 								 								
	 								vertX, vertY = vs.GetPolyPt(h, 1)
	 								if("{:.6f}".format(vertX) == "{:.6f}".format(txtXCoordinate) and "{:.6f}".format(vertY) == "{:.6f}".format(txtYCoordinate)):	 									

	 									numofVertices = vs.GetVertNum(h)
	 									
	 									patValue = vs.GetFPat(h)
	 									redBackVal, greenBackVal, blueBackVal = vs.GetFillBack(h)
	 									redForeVal, greenForeVal, blueForeVal = vs.GetFillFore(h)
	 									
	 									if(vs.IsPolyClosed(h)):
	 										vs.ClosePoly()
	 									vs.DelObject(h)
	 									vs.BeginPoly3D()
	 									vs.Add3DPt(txtXCoordinate, txtYCoordinate, txtZCoordinate)
	 									for currVertx in itertools.islice(pointIterator, numofVertices - 1):
	 										for currXYPoint in currVertx.iter('Point'):
		 										txtLonCoordinate, txtLatCoordinate, alaki = currXYPoint.find('coordinates').text.strip().split(',')
		 										txtZCoordinate = float(currPoint.find('name').text)
		 										isValid, tempo = vs.GeogCoordToVW(float(txtLatCoordinate), float(txtLonCoordinate))
		 										txtXCoordinate = tempo[0]
		 										txtYCoordinate = tempo[1]
		 										vs.Add3DPt(txtXCoordinate, txtYCoordinate, txtZCoordinate)
 										vs.EndPoly3D()
 										list_of_processedObjects.append(vs.LNewObj())
 										numofSelectedPoints += 1
 										break
	
	
	 						h = vs.NextObj(h);
	 					else:
	 						hLayer = vs.NextLayer(hLayer);
	 						continue
	 					break
	 					 					
		vs.AlrtDialog(str(numofSelectedPoints) + ' Points have been updated and selected!')
				
execute()
```

## See Also

Python basic information: [Python](../README.md)

[Script Function Reference](../../Function%20Reference/README.md)

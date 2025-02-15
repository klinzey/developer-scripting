# BuildResourceList

## Description
Creates an implicit list of  resources of a specified type, and returns an ID for the list. Values in the list can be retrieved using GetNameFromResourceList.&lt;BR&gt;
&lt;BR&gt;
If the Display Default Content preference (#130) is on and folderIndex is not  0, it will also include all the resources of the specified type in all the files in the selected folder. &lt;BR&gt;
&lt;BR&gt;
If folderIndex is positive, the list will include all the resources of that type from the current document, as well as from the specified folder. If folderIndex is 0, only the resources in the current document will be in the list. If folderIndex is negative, only the resources in the specified folder will be in the list.   &lt;BR&gt;
&lt;BR&gt;
A complete listing of supported object types may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#objects&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Folder Path Selectors&lt;/I&gt;
&lt;P&gt; 
&lt;CENTER&gt;
  &lt;TABLE WIDTH=300 ALIGN=CENTER&gt;
   &lt;TR&gt;
    &lt;TD&gt;
     &lt;B&gt;&lt;I&gt; Note that use of the negative values of these constants can be used to get the user-based folder path.  The positive values are for application-based paths, which should not be used for writing. &lt;/I&gt;&lt;/B&gt;
    &lt;/TD&gt;
   &lt;/TR&gt;
  &lt;/TABLE&gt;
  &lt;P&gt;
  &lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
    &lt;TR&gt; 
      &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF &gt;Folder Name&lt;/FONT&gt;&lt;/TH&gt;
      &lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF &gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Application&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plug-Ins&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Workspaces&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Templates&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;7&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Standards&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;8&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Help&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;9&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Dictionaries&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;10&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;User App Data&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;12&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Libraries&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;13&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Defaults&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;14&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Settings&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;15&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;PDF Resources&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;18&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plug-In Data&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;20&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plug-In Includes&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;21&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plug-In interfaces&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;22&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Favorites&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;23&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Renderworks - Textures&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;100&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Cabinet - Handles&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;101&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Door - Hardware&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;102&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Attributes - Gradients&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;103&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Hardscape - Hatches&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;104&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Attributes - Hatches&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;105&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Attributes - Image Fills&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;106&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plants&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;107&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Toilet Stall - Fixtures&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;108&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;RenderWorks - Backgrounds&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;109&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Seating Layout - Symbols&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;110&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Tile - Symbols&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;111&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Human Figure - Textures&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;112&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Walls&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;113&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Stairs&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;114&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Drawing Border - Title Blocks&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;115&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Section - Markers&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;116&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;117&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Door - Custom Leaves&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;118&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Lighting Instrument - Gobos&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;119&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Reports~Schedules&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;120&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Lighting Instrument - Symbols&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;121&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plants - Hatches&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;124&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Flooring/Decking&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;125&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Framing&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;126&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Masonry Units&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;127&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Miscellaneous&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;128&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Roofing&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;129&lt;/TD&gt;
    &lt;/TR&gt;
	&lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Repetitive Unit: Siding&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;130&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Walls - Hatches&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;131&lt;/TD&gt;
    &lt;/TR&gt;
    &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Walls - Textures&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;132&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Window - Custom Shutters&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;133&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Sketch Styles&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;134&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Plant Database&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;135&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;VW Plants&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;136&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Color Palettes&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;137&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Framing Member - Custom Profile&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;138&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Spaces - Occupant Organization Name Lists&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;140&lt;/TD&gt;
    &lt;/TR&gt;
     &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Spaces - Space Name Lists and Libraries&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;141&lt;/TD&gt;
    &lt;/TR&gt;
	 &lt;TR&gt; 
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Structural Shapes&lt;/TD&gt;
      &lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;142&lt;/TD&gt;
    &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
FUNCTION BuildResourceList(
				type          : INTEGER;
				folderIndex   : INTEGER;
				subFolderName : DYNARRAY[] of CHAR;
				VAR numItems  : LONGINT) : LONGINT;
```

```python

def vs.BuildResourceList(type, folderIndex, subFolderName):
    return (LONGINT, numItems)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|type|INTEGER|the type of resource to put in the list|
|folderIndex|INTEGER|the index of a VW folder. |
|subFolderName|DYNARRAY[] of CHAR|the name of a subfolder inside the folder specified by folderIndex. This can also be a partial path.  Use an empty string to request the resources from all files in the folderIndex folder.|
|numItems|LONGINT|the number of items in the list built|

## Examples
```pascal
const

kHatch = 66;

kDefHatchFolder = 105;

var

listID, numItems: LONGINT;

begin

{ Create a resource list of hatches from the current document and } 

{ the default hatch folder. }

listID := BuildResourceList(kHatch, kDefHatchFolder, '', numItems);


```

## See Also
VS Functions:
[AddResourceToList](AddResourceToList.md)| [DeleteResourceFromList](DeleteResourceFromList.md)| [GetNameFromResourceList](GetNameFromResourceList.md)| [GetResourceFromList](GetResourceFromList.md)| [ImportResourceToCurrentFile](ImportResourceToCurrentFile.md)

## Version
Availability: from VectorWorks12.0
## Category
* Document List Handling


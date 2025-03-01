## How to install
Create a new Vectorworks document and add a new Script resource in the resource browser.
Use the text below for the script and make sure you select Python language.

## How the sample works

```py
import os

major, minor, maintenance, platform = vs.GetVersion()
isMac = False
if platform == 1: isMac = True

# define a location to import the images
importPt = (0,0)

symCreatedCnt = 0

err, dirPath = vs.GetFolder('Select a Folder')
if err == 0: # no-error
    hsfDirPath = dirPath
    if isMac: ok, hsfDirPath = vs.ConvertPosix2HSFPath(dirPath)

    fileIndex = 1
    while True: # loop the files
        fileName = vs.GetFilesInFolder(hsfDirPath, fileIndex)
        fileIndex += 1

        if fileName == '': # no more files
            break

        name, ext = os.path.splitext(fileName)
        if ext.lower() == '.png' or ext.lower() == '.jpg':
            imagePath = os.path.join(dirPath, fileName)

            vs.BeginSym(name)
            hImage = vs.ImportImageFile(imagePath, importPt)
            vs.EndSym()
            symCreatedCnt += 1

vs.AlrtDialog('Done! Created ', symCreatedCnt, ' symbols.')
```

## See Also

Python basic information: [Python](../README.md)

[Script Function Reference](../../Function%20Reference/README.md)

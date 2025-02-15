# FindFile

## Description
Find a file by searching the folder selector (whichPath) plus the relative file path. Searches the user folder, workgroup folders, and the app folder.

```pascal
FUNCTION FindFile(
				whichPath   : INTEGER;
				relFilePath : DYNARRAY[] of CHAR;
				VAR outPath : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.FindFile(whichPath, relFilePath):
    return (BOOLEAN, outPath)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|whichPath|INTEGER||
|relFilePath|DYNARRAY[] of CHAR||
|outPath|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2015
## Category
* File I/O


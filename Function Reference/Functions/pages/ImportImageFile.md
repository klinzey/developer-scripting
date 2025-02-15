# ImportImageFile

## Description
Import the specified image file as an Image object in Vectorworks.

```pascal
FUNCTION ImportImageFile(
				filePath : DYNARRAY[] of CHAR;
				importPt : REAL) : HANDLE;
```

```python

def vs.ImportImageFile(filePath, importPt):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filePath|DYNARRAY[] of CHAR|Full path to the image file.|
|importPt|REAL|Location on which the file should be imported.|

## Version
Availability: from Vectorworks 2014
## Category
* Utility


# GetWallHoleTexturePart

## Description
Gets the wall texture part of an object in the wall hole group of a symbol definition or plug-in object.  This is the wall texture part given to faces of the wall that are created by cutting a hole in the wall with the object.

```pascal
FUNCTION GetWallHoleTexturePart(object : HANDLE) : INTEGER;
```

```python

def vs.GetWallHoleTexturePart(object):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The handle to the cutting object in the wall hole group of a symbol definition or plug-in object.|

## Returns
The wall texture part.<BR>
<BR>
0 - The wall Holes texture part<BR>
1 - The wall Left texture part<BR>
2 - The wall Right texture part

## See Also
VS Functions:
[SetWallHoleTexturePart](SetWallHoleTexturePart.md)

## Version
Availability: from Vectorworks 2010
## Category
* Textures


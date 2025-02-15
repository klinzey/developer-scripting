# SetComponentWallBottomOffset

## Description
Sets the offset from wall bottom of a component in an object.

```pascal
FUNCTION SetComponentWallBottomOffset(
				object               : HANDLE;
				componentIndex       : INTEGER;
				offsetFromWallBottom : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetComponentWallBottomOffset(object, componentIndex, offsetFromWallBottom):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|
|componentIndex|INTEGER|The index of the component.|
|offsetFromWallBottom|REAL (Coordinate)|The offset from wall bottom of the component.|

## See Also
VS Functions:
[GetComponentWallBottomOffset](GetComponentWallBottomOffset.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


# SetComponentWallTopOffset

## Description
Sets the offset from wall top of a component in an object.

```pascal
FUNCTION SetComponentWallTopOffset(
				object            : HANDLE;
				componentIndex    : INTEGER;
				offsetFromWallTop : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetComponentWallTopOffset(object, componentIndex, offsetFromWallTop):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|
|componentIndex|INTEGER|The index of the component.|
|offsetFromWallTop|REAL (Coordinate)|The offset from wall top of the component.|

## See Also
VS Functions:
[GetComponentWallTopOffset](GetComponentWallTopOffset.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


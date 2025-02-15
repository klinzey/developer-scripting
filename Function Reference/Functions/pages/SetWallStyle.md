# SetWallStyle

## Description
Applies the given Wall Style to the given wall, aligning to the given offsets.

```pascal
FUNCTION SetWallStyle(
				theWall              : HANDLE;
				wallStyle            : STRING;
				selectedOffDistance  : REAL (Coordinate);
				replacingOffDistance : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetWallStyle(theWall, wallStyle, selectedOffDistance, replacingOffDistance):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall.|
|wallStyle|STRING|The Wall Style to apply.|
|selectedOffDistance|REAL (Coordinate)|The offset of the wall to align to.|
|replacingOffDistance|REAL (Coordinate)|The offset of the Wall Style to align to.|

## Returns
Returns success status.

## See Also
VS Functions:
[GetWallStyle](GetWallStyle.md)

## Version
Availability: from VectorWorks12.5
## Category
* Objects - Walls


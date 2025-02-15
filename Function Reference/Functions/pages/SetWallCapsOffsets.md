# SetWallCapsOffsets

## Description
Set the wall's caps' offsets.

```pascal
FUNCTION SetWallCapsOffsets(
				theWall               : HANDLE;
				leftCapLeftDistance   : REAL (Coordinate);
				leftCapRightDistance  : REAL (Coordinate);
				rightCapLeftDistance  : REAL (Coordinate);
				rightCapRightDistance : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetWallCapsOffsets(theWall, leftCapLeftDistance, leftCapRightDistance, rightCapLeftDistance, rightCapRightDistance):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall.|
|leftCapLeftDistance|REAL (Coordinate)|The left offset of the left wall cap.|
|leftCapRightDistance|REAL (Coordinate)|The right offset of the left wall cap.|
|rightCapLeftDistance|REAL (Coordinate)|The left offset of the right wall cap.|
|rightCapRightDistance|REAL (Coordinate)|The right offset of the right wall cap.|

## Returns
Returns success status.

## See Also
VS Functions:
[GetWallCapsOffsets](GetWallCapsOffsets.md)

## Version
Availability: from VectorWorks12.5
## Category
* Objects - Walls


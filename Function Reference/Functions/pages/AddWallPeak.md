# AddWallPeak

## Description
Procedure AddWallPeak creates a wall peak in the referenced wall object.

```pascal
PROCEDURE AddWallPeak(
				wallHd         : HANDLE;
				offDistance    : REAL (Coordinate);
				heightDistance : REAL (Coordinate));
```

```python

def vs.AddWallPeak(wallHd, offDistance, heightDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallHd|HANDLE|Handle to wall.|
|offDistance|REAL (Coordinate)|Offset distance from wall start.|
|heightDistance|REAL (Coordinate)|Elevation of wall peak.|

## Version
Availability: from MiniCAD6.0
## Category
* Objects - Walls


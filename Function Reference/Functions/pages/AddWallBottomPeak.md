# AddWallBottomPeak

## Description
Adds a peak to the bottom of the referenced wall.

```pascal
PROCEDURE AddWallBottomPeak(
				wallHd         : HANDLE;
				offDistance    : REAL (Coordinate);
				heightDistance : REAL (Coordinate));
```

```python

def vs.AddWallBottomPeak(wallHd, offDistance, heightDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallHd|HANDLE|Handle to wall.|
|offDistance|REAL (Coordinate)|Offset distance of peak from wall start.|
|heightDistance|REAL (Coordinate)|Height of peak.|

## Examples
```pascal
AddWallBottomPeak(h,24'0&quot;,2'6&quot;);
```

## Version
Availability: from VectorWorks9.0
## Category
* Objects - Walls


# OffsetPolyN

## Description
Offsets a polygon or polyline. Uses Parasolid to do it. Equivalent of Voronoy based OffsetPoly.

```pascal
FUNCTION OffsetPolyN(
				h              : HANDLE;
				offsetDistance : REAL;
				smoothCorners  : BOOLEAN) : HANDLE;
```

```python

def vs.OffsetPolyN(h, offsetDistance, smoothCorners):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|offsetDistance|REAL||
|smoothCorners|BOOLEAN||

## Version
Availability: from Vectorworks 2014
## Category
* Graphic Calculation


# PointAlongPoly

## Description
Returns a point at the specified distance along the poly, and a vector tangent to the poly at that point.

```pascal
FUNCTION PointAlongPoly(
				h           : HANDLE;
				dist        : REAL;
				VAR pt      : VECTOR;
				VAR tangent : VECTOR) : BOOLEAN;
```

```python

def vs.PointAlongPoly(h, dist):
    return (BOOLEAN, pt, tangent)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|dist|REAL||
|pt|VECTOR||
|tangent|VECTOR||

## Version
Availability: from Vectorworks 2014
## Category
* Graphic Calculation


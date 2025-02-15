# SetPolyPt3D

## Description
Procedure SetPolyPt3D sets the position of the specified vertex in the referenced 3D object.&lt;BR&gt;


```pascal
PROCEDURE SetPolyPt3D(
				objectHd : HANDLE;
				index    : INTEGER;
				p        : REAL;
				zValue   : REAL);
```

```python

def vs.SetPolyPt3D(objectHd, index, p, zValue):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to mesh or 3D poly object.|
|index|INTEGER|Index of vertex point.|
|p|REAL|New X-Y coordinates of vertex.|
|zValue|REAL|New elevation of vertex.|

## Examples
```pascal
SetPolyPt3D(objectHandle,3,2.5&quot;,3&quot;,8&quot;);
```

## Version
Availability: from MiniCAD7.0
## Category
* Objects - 3D


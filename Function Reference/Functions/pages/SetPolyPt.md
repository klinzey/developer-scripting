# SetPolyPt

## Description
Procedure SetPolyPt sets the location a specified vertex in the referenced polygon or polyline.&lt;BR&gt;


```pascal
PROCEDURE SetPolyPt(
				objectHd : HANDLE;
				index    : INTEGER;
				xR       : REAL;
				yR       : REAL);
```

```python

def vs.SetPolyPt(objectHd, index, xR, yR):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to polygon.|
|index|INTEGER|Index of vertex.|
|xR|REAL|New X coordinate of vertex.|
|yR|REAL|New Y coordinate of vertex.|

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


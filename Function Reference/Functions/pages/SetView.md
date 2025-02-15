# SetView

## Description
Procedure SetView sets the view of a Vectorworks document. The projection must be non-plan to modify the view.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetView(
				xAngle    : REAL;
				yAngle    : REAL;
				zAngle    : REAL;
				xDistance : REAL (Coordinate);
				yDistance : REAL (Coordinate);
				zDistance : REAL (Coordinate));
```

```python

def vs.SetView(xAngle, yAngle, zAngle, xDistance, yDistance, zDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|xAngle|REAL|X axis rotation angle.|
|yAngle|REAL|Y axis rotation angle.|
|zAngle|REAL|Z axis rotation angle.|
|xDistance|REAL (Coordinate)|X coordinate of view center.|
|yDistance|REAL (Coordinate)|Y coordinate of view center.|
|zDistance|REAL (Coordinate)|Z coordinate of view center.|

## Examples
```pascal
SetView(45d,30d,30d,0,2,2);


```

## Version
Availability: from MiniCAD
## Category
* View / Zoom


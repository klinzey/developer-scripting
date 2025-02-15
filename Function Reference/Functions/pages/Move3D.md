# Move3D

## Description
Procedure Move3D moves the most recently created three-dimensional object a relative distance from it's original location. The object is moved relative to its center. &lt;BR&gt;


```pascal
PROCEDURE Move3D(
				xDistance : REAL (Coordinate);
				yDistance : REAL (Coordinate);
				zDistance : REAL (Coordinate));
```

```python

def vs.Move3D(xDistance, yDistance, zDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|xDistance|REAL (Coordinate)|X offset distance.|
|yDistance|REAL (Coordinate)|Y offset distance.|
|zDistance|REAL (Coordinate)|Z offset ditance.|

## Examples
```pascal
BeginXtrd(0',2&quot;);

Rect(0&quot;,1&quot;,1&quot;,0&quot;);

EndXtrd;

Move3D(3&quot;,1&quot;,2&quot;);


```

## Version
Availability: from MiniCAD
## Category
* Object Editing


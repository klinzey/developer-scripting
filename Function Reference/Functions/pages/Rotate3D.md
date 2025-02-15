# Rotate3D

## Description
Procedure Rotate3D rotates the most recently created three-dimensional object. Rotation values are applied about the respective axes.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Rotate3D(
				xAngle : REAL;
				yAngle : REAL;
				zAngle : REAL);
```

```python

def vs.Rotate3D(xAngle, yAngle, zAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|xAngle|REAL|Rotation about X-axis.|
|yAngle|REAL|Rotation about Y-axis|
|zAngle|REAL|Rotation about Z-axis.|

## Examples
```pascal
BeginXtrd(0&quot;,4&quot;);

Rect(0&quot;,3&quot;,1&quot;,0&quot;);

EndXtrd;

Rotate3D(21d 10' 22&quot;,-18d 44' 50&quot;,-7d 5' 45&quot;);


```

## Version
Availability: from MiniCAD
## Category
* General Edit


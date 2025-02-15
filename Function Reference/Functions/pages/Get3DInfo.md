# Get3DInfo

## Description
Procedure Get3DInfo returns the height, width and depth values of the referenced 3D object.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Get3DInfo(
				h          : HANDLE;
				VAR height : REAL;
				VAR width  : REAL;
				VAR depth  : REAL);
```

```python

def vs.Get3DInfo(h):
    return (height, width, depth)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to 3D object.|
|height|REAL|Height of object.|
|width|REAL|Width of object.|
|depth|REAL|Depth of object.|

## Examples
```pascal
PROCEDURE GetBBox3D(h :HANDLE; VAR x1, y1, z1, x2, y2, z2 :REAL);

VAR

	garb_r, z_span, z_center :REAL;

BEGIN

	GetBBox(h, x1, y1, x2, y2);

	Get3DInfo(h, garb_r, garb_r, z_span);

	Get3DCntr(h, garb_r, garb_r, z_center);

	z1 := z_center - (z_span / 2);

	z2 := z_center + (z_span / 2);

END;


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


# RotatePoint

## Description
Procedure RotatePoint rotates selected Vectorworks objects about the specified coordinate point.

```pascal
PROCEDURE RotatePoint(
				p             : REAL;
				rotationAngle : REAL);
```

```python

def vs.RotatePoint(p, rotationAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Point of rotation.|
|rotationAngle|REAL|Rotation angle.|

## Examples
```pascal
SetSelect(LNewObj);

RotatePoint(0,3,45d);


```

## Version
Availability: from MiniCAD6.0
## Category
* General Edit


# SetWorkingPlane

## Description
Sets the x, y, and z offset of the working plane as well as the x-, y-, and z-plane rotational values.

```pascal
PROCEDURE SetWorkingPlane(
				x         : REAL;
				y         : REAL;
				z         : REAL;
				xRotation : REAL;
				yRotation : REAL;
				zRotation : REAL);
```

```python

def vs.SetWorkingPlane(x, y, z, xRotation, yRotation, zRotation):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|x|REAL|X-coordinate of the working plane|
|y|REAL|Y-coordinate of the working plane|
|z|REAL|Z-coordinate of the working plane|
|xRotation|REAL|X-coordinate of the rotation|
|yRotation|REAL|Y-coordinate of the rotation|
|zRotation|REAL|Z-coordinate of the rotation|

## See Also
VS Functions:
[GetWorkingPlane](GetWorkingPlane.md)

## Version
Availability: from VectorWorks10.0
## Category
* Utility


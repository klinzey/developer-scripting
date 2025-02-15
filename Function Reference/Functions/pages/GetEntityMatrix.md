# GetEntityMatrix

## Description
Gets the matrix of the plane for a planar object.

```pascal
FUNCTION GetEntityMatrix(
				objectHandle       : HANDLE;
				VAR offset         : REAL;
				VAR rotationXAngle : REAL;
				VAR rotationYAngle : REAL;
				VAR rotationZAngle : REAL) : BOOLEAN;
```

```python

def vs.GetEntityMatrix(objectHandle):
    return (BOOLEAN, offset, rotationXAngle, rotationYAngle, rotationZAngle)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|The object for which the matrix of its plane is being obtained.|
|offset|REAL|The offset of the plane in current document units.|
|rotationXAngle|REAL|The rotation of the plane about the X-axis in degrees.|
|rotationYAngle|REAL|The rotation of the plane about the Y-axis in degrees.|
|rotationZAngle|REAL|The rotation of the plane about the Z-axis in degrees.|

## Returns
Returns true if the object passed is a planar object.

## Version
Availability: from Vectorworks 2011
## Category
* Object Attributes


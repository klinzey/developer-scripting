# Centroid3D

## Description
Returns the center of gravity of a 3D object. The function returns TRUE if the values were found.

```pascal
FUNCTION Centroid3D(
				object  : HANDLE;
				VAR xCG : REAL;
				VAR yCG : REAL;
				VAR zCG : REAL) : BOOLEAN;
```

```python

def vs.Centroid3D(object):
    return (BOOLEAN, xCG, yCG, zCG)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The objectt from whci to calculate the center of gravity|
|xCG|REAL|The x component of the center of gravity.|
|yCG|REAL|The y component of the center of gravity.|
|zCG|REAL|The z component of the center of gravity.|

## Returns
Returns true if the function succeeds.

## Version
Availability: from VectorWorks10.1
## Category
* Objects - 3D


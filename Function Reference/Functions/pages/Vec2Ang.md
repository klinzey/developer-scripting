# Vec2Ang

## Description
Returns the angle, in degrees, of the specified vector. If Vect is a 3D vector, Vec2Ang will return the 3D angle between Vect and the X axis. If Vect is {0,0,0}, Vec2Ang returns -90.&lt;BR&gt;


```pascal
FUNCTION Vec2Ang(Vect : VECTOR) : REAL;
```

```python

def vs.Vec2Ang(Vect):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|Vect|VECTOR|Source vector.|

## Returns
Returns the angle of the specified vector in degrees.

## Version
Availability: from MiniCAD
## Category
* Math - Vectors


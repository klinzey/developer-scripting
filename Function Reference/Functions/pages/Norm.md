# Norm

## Description
Returns the length, or magnitude, of the specified vector.

```pascal
FUNCTION Norm(Vec : VECTOR) : REAL;
```

```python

def vs.Norm(Vec):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|Vec|VECTOR|Vector to be measured.|

## Returns
A REAL value which is the length of the vector.

## Examples
```pascal
PROCEDURE Example;

VAR

	vec :VECTOR;

BEGIN

	vec.x := 1;

	vec.y := 1.732050807;

	Message(Norm(vec));

END;

RUN(Example);
```

## See Also
VS Functions:
[Distance](Distance.md)

## Version
Availability: from MiniCAD
## Category
* Math - Vectors


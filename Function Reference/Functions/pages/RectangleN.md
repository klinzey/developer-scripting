# RectangleN

## Description
Creates and returns a handle to a new rectangle object with the specified bounds.

```pascal
PROCEDURE RectangleN(
				orgin     : REAL;
				direction : REAL;
				width     : REAL;
				height    : REAL);
```

```python

def vs.RectangleN(orgin, direction, width, height):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|orgin|REAL||
|direction|REAL||
|width|REAL||
|height|REAL||

## Examples
```pascal
PROCEDURE Example;

BEGIN

	RectangleN(0, 0, 1, 0, 1, 1);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks 2008
## Category
* Objects - 2D


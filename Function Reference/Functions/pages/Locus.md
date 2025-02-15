# Locus

## Description
Procedure Locus creates a 2D locus object at the specified coordinate location. &lt;BR&gt;


```pascal
PROCEDURE Locus(p : REAL);
```

```python

def vs.Locus(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Coordinate location of new locus.|

## Examples
```pascal
PROCEDURE Example;

VAR

	x, y :REAL;

BEGIN

	HCenter(FSActLayer, x, y);

	Locus(x, y);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


# EqualPt

## Description
Function EqualPt returns whether the two specified coordinate locations are equal (i.e., the same point, to 12 significant digits).&lt;BR&gt;


```pascal
FUNCTION EqualPt(
				p1 : REAL;
				p2 : REAL) : BOOLEAN;
```

```python

def vs.EqualPt(p1, p2):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Coordinates of first comparison point.|
|p2|REAL|Coordinates of second comparison point.|

## Examples
```pascal
PROCEDURE Example;

VAR

	x1, y1, x2, y2 :REAL;

BEGIN

	x1 := 1;

	y1 := 1;

	x2 := 1.0000000000001;

	y2 := 1.0000000000001;

	Message(EqualPt(x1, y1, x2, y2));

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Graphic Calculation


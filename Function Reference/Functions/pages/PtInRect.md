# PtInRect

## Description
Function PtInRect returns whether the coordinate location is located within the specified rectangular boundary.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION PtInRect(
				point : REAL;
				rect1 : REAL;
				rect2 : REAL) : BOOLEAN;
```

```python

def vs.PtInRect(point, rect1, rect2):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|point|REAL|X-Y coordinate point location.|
|rect1|REAL|Top left coordinate of rectangular area.|
|rect2|REAL|Bottom right coordinate of rectangular area.|

## Examples
```pascal
PROCEDURE Example;

VAR

	pointX, pointY, rect1X, rect1Y, rect2X, rect2Y :REAL;

BEGIN

	pointX := 1;

	pointY := 1;

	rect1X := 0;

	rect1Y := 2;

	rect2X := 2;

	rect2Y := 0;

	Message(PtInRect(pointX, pointY, rect1X, rect1Y, rect2X, rect2Y));

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Graphic Calculation


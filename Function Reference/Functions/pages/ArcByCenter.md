# ArcByCenter

## Description
Creates an arc using a center point, the radius, a start angle, and a sweep.

```pascal
PROCEDURE ArcByCenter(
				x          : REAL;
				y          : REAL;
				radius     : REAL;
				startAngl  : REAL;
				sweepAngle : REAL);
```

```python

def vs.ArcByCenter(x, y, radius, startAngl, sweepAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|x|REAL|X-coordinate of the center point|
|y|REAL|Y-coordinate of the center point|
|radius|REAL|Radius of the arc|
|startAngl|REAL|Starting angle of the arc|
|sweepAngle|REAL|Sweep angle of the arc|

## Examples
```pascal
PROCEDURE Example;

VAR

	x, y, radius, startAngle, sweepAngle :REAL;

BEGIN

	GetPt(x, y);

	radius := 3;

	startAngle := 0;

	sweepAngle := 90;

	ArcByCenter(x, y, radius, startAngle, sweepAngle);

	AlrtDialog(Concat(GetType(LNewObj)));

END;

RUN(Example);
```

## Version
Availability: from VectorWorks10.0
## Category
* Objects - 2D


# GetArc

## Description
Procedure GetArc returns the start and sweep angle of the referenced arc or round wall.

```pascal
PROCEDURE GetArc(
				h               : HANDLE;
				VAR startAngleR : REAL;
				VAR arcAngleR   : REAL);
```

```python

def vs.GetArc(h):
    return (startAngleR, arcAngleR)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to arc.|
|startAngleR|REAL|Returns start angle of arc.|
|arcAngleR|REAL|Returns sweep angle of arc.|

## Examples
```pascal
PROCEDURE GetArcSetArcExample;

VAR

	h :HANDLE;

	startAng, sweepAng :REAL;

BEGIN

	h := FSActLayer;

	GetArc(h, startAng, sweepAng);

	SetArc(h, startAng, sweepAng + 10);

END;

RUN(GetArcSetArcExample);
```

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


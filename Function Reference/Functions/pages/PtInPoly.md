# PtInPoly

## Description
Function PtInPoly returns TRUE if the point specified point lies within, or on, the referenced polygon or polyline object.

```pascal
FUNCTION PtInPoly(
				p : REAL;
				h : HANDLE) : BOOLEAN;
```

```python

def vs.PtInPoly(p, h):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|X-Y coordinate point.|
|h|HANDLE|Handle to polygon.|

## Examples
```pascal
PROCEDURE Example;

VAR

	polyHandle :HANDLE;

	locusHandle :HANDLE;

	x, y :REAL;

BEGIN

	CallTool(-204); polyHandle := FSActLayer;

	CallTool(-221); locusHandle := FSActLayer;

	GetLocPt(locusHandle, x, y);

	Message(PtInPoly(x, y, polyHandle));

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Graphic Calculation


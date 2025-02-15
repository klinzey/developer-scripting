# GetObjArrow

## Description
Procedure GetObjArrow returns the arrow style parameters for the indicated object.&lt;BR&gt;


```pascal
PROCEDURE GetObjArrow(
				obj       : HANDLE;
				VAR style : INTEGER;
				VAR size  : REAL;
				VAR angle : INTEGER;
				VAR start : BOOLEAN;
				VAR end   : BOOLEAN);
```

```python

def vs.GetObjArrow(obj):
    return (style, size, angle, start, end)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|The indicated object.|
|style|INTEGER|Returns arrow style.|
|size|REAL|Returns arrow size in inches measured in page space.|
|angle|INTEGER|Returns arrow angle (in degrees).|
|start|BOOLEAN|Returns whether the start point of the object has an arrow.|
|end|BOOLEAN|Returns whether the endpoint of the object has an arrow.|

## Remarks
OBSOLETE for VW2008: Use GetObjBeginningMarker and/or GetObjEndMarker instead.<BR>
Style indicates the index of the arrow style to be used.<BR>
<BR>
Size is in page-inches. Legal values are 0.0 to 2.0.<BR>
<BR>
Angle is in degrees.

## Examples
```pascal
PROCEDURE ShowObjArrowValues;

VAR

	style :INTEGER;

	size	 :REAL;

	ang	 :INTEGER;

	start :BOOLEAN;

	endPt :BOOLEAN;

	obj   :HANDLE;

BEGIN

	obj := FSActLayer;

	GetObjArrow(obj, style, size, ang, start, endPt);

	Message(style, ' ', size, ' ', ang, ' ', start, ' ', endPt);

END;

RUN(ShowObjArrowValues);
```

## Version
```diff
- GetObjArrow is obsolete as of VectorWorks 2008
```

Availability: from VectorWorks10.0
## Category
* Object Attributes


# GetClassArrow

## Description
Procedure GetClassArrow returns the arrow style parameters for the indicated class.&lt;BR&gt;


```pascal
PROCEDURE GetClassArrow(
				className : STRING;
				VAR style : INTEGER;
				VAR size  : REAL;
				VAR angle : INTEGER);
```

```python

def vs.GetClassArrow(className):
    return (style, size, angle)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|The indicated class.|
|style|INTEGER|Returns arrow style.|
|size|REAL|Returns arrow size in inches measured in page space.|
|angle|INTEGER|Returns arrow angle (in degrees).|

## Remarks
OBSOLETE for VW2008: Use GetClassBeginningMarker and/or GetClassEndMarker instead.<BR>
Style indicates the index of the arrow style to be used.<BR>
<BR>
Size is in page-inches. Legal values are 0.0 to 2.0.<BR>
<BR>
Angle is in degrees.

## Examples
```pascal
PROCEDURE ShowNoneClassArrowValues;

VAR

	style :INTEGER;

	size  :REAL;

	ang   :INTEGER;

BEGIN

	GetClassArrow('None', style, size, ang);

	Message(style, ' ', size, ' ', ang);

END;

RUN(ShowNoneClassArrowValues);
```

## Version
```diff
- GetClassArrow is obsolete as of VectorWorks 2008
```

Availability: from VectorWorks10.0
## Category
* Classes


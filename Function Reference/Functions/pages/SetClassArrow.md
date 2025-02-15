# SetClassArrow

## Description
Procedure SetClassArrow sets the arrow style parameters for the indicated class.&lt;BR&gt;


```pascal
PROCEDURE SetClassArrow(
				className : STRING;
				style     : INTEGER;
				size      : REAL;
				angle     : INTEGER);
```

```python

def vs.SetClassArrow(className, style, size, angle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|The indicated class.|
|style|INTEGER|The arrow style.|
|size|REAL|The arrow size in inches measured in page space.|
|angle|INTEGER|The arrow angle (in degrees).|

## Remarks
OBSOLETE for VW2008: Use SetClassBeginningMarker and/or SetClassEndMarker instead.<BR>
Style indicates the index of the arrow style to be used.<BR>
<BR>
Size is in page-inches. Legal values are 0.0 to 2.0.<BR>
<BR>
Angle is in degrees.

## Examples
```pascal
SetClassArrow('None', 2, 0.25, 15);


```

## Version
```diff
- SetClassArrow is obsolete as of VectorWorks 2008
```

Availability: from VectorWorks10.0
## Category
* Classes


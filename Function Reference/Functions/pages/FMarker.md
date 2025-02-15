# FMarker

## Description
Procedure FMarker returns the active marker style parameters.&lt;BR&gt;
&lt;BR&gt;
A complete listing of marker styles can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#marker&quot;&gt;Appendix&lt;/A&gt;


```pascal
PROCEDURE FMarker(
				VAR style : INTEGER;
				VAR size  : REAL;
				VAR ang   : INTEGER);
```

```python

def vs.FMarker():
    return (style, size, ang)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|style|INTEGER|Returns marker style.|
|size|REAL|Returns marker size in inches measured in page space.|
|ang|INTEGER|Returns marker angle (in degrees).|

## Remarks
OBSOLETE for VW2008: Use GetDefaultBeginningMarker and/or GetDefaultEndMarker instead.<BR>
Style is an 8 bit quantity interpreted as follows:<BR>
<BR>
Bit 0 indicates the visibility of a marker at the start of the line.<BR>
Bit 1 indicates the visibility of a marker at the end of the line.<BR>
Bits 2 - 7 indicate the index of the marker style to be used.<BR>
<BR>
Size is in page-inches. Legal values are 0.0 to 2.0.<BR>
<BR>
Angle is in degrees.<BR>
[sd 8/14/98]

## Examples
```pascal
PROCEDURE Example;

VAR

	style :INTEGER;

	size  :REAL;

	ang   :INTEGER;

BEGIN

	FMarker(style, size, ang);

	Message(style, ' ', size, ' ', ang);

END;

RUN(Example);




```

## Version
```diff
- FMarker is obsolete as of VectorWorks 2008
```

Availability: from MiniCAD6.0
## Category
* Document Attributes


# SetObjArrow

## Description
Procedure SetObjArrow sets the arrow style parameters for the indicated object.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Marker Styles&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Marker 
	  Style&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Filled Arrow&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Empty Arrow&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Open Arrow&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Filled Circle&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Empty Circle&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Slash&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Cross&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetObjArrow(
				obj   : HANDLE;
				style : INTEGER;
				size  : REAL;
				angle : INTEGER;
				start : BOOLEAN;
				end   : BOOLEAN);
```

```python

def vs.SetObjArrow(obj, style, size, angle, start, end):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|The indicated object.|
|style|INTEGER|The arrow style.|
|size|REAL|The arrow size in inches measured in page space.|
|angle|INTEGER|The arrow angle (in degrees).|
|start|BOOLEAN|Whether the start point of the object has an arrow.|
|end|BOOLEAN|Whether the endpoint of the object has an arrow.|

## Remarks
OBSOLETE for VW2008: Use SetObjBeginningMarker and/or SetObjEndMarker instead.<BR>
Style indicates the index of the arrow style to be used.<BR>
<BR>
Size is in page-inches. Legal values are 0.0 to 2.0.<BR>
<BR>
Angle is in degrees.

## Examples
```pascal
PROCEDURE SetObjArrowValues;

BEGIN

	SetObjArrow(FSActLayer, 1, .25, 15, TRUE, TRUE);

END;

RUN(SetObjArrowValues);
```

## Version
```diff
- SetObjArrow is obsolete as of VectorWorks 2008
```

Availability: from VectorWorks10.0
## Category
* Object Attributes


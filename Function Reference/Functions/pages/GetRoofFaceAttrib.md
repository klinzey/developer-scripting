# GetRoofFaceAttrib

## Description
Returns information on the referenced roof face object.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Roof Miter Styles&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Miter Style&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Constant&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Vertical&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Horizontal&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Double&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;&lt;p&gt;3&lt;/p&gt;&lt;/TD&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Square&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;&lt;p&gt;4&lt;/p&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE GetRoofFaceAttrib(
				roofFace      : HANDLE;
				VAR roofRise  : REAL;
				VAR roofRun   : REAL;
				VAR miterType : INTEGER;
				VAR holeStyle : INTEGER;
				VAR vertPart  : REAL;
				VAR thickness : REAL);
```

```python

def vs.GetRoofFaceAttrib(roofFace):
    return (roofRise, roofRun, miterType, holeStyle, vertPart, thickness)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofFace|HANDLE|Handle to roof face object.|
|roofRise|REAL|Rise of roof.|
|roofRun|REAL|Run of roof.|
|miterType|INTEGER|Miter style of roof.|
|holeStyle|INTEGER|Miter style of openings.|
|vertPart|REAL|Vertical component of compound miters.|
|thickness|REAL|Thickness of roof.|

## Remarks
Returns information about old-style roof objects (single roof faces).<BR>
<BR>
Returns slope, edge miter style, miter dimensions, and thickness of roof object.<BR>
<BR>
See Also GetRoofFaceCoord() for additional roof face data

## Examples
```pascal
PROCEDURE Example;



PROCEDURE ShowRoofFaceAttrib(roofFace :HANDLE);

VAR

	roofRise, roofRun :REAL; 

	miterType, holeStyle :INTEGER; 

	vertPart, thickness :REAL;

BEGIN

	IF GetObjectVariableInt(roofFace, 172) = 1 THEN BEGIN

		GetRoofFaceAttrib(roofFace, roofRise, roofRun, miterType, holeStyle, vertPart, thickness);

		Message('roofRise: ', roofRise,

			',  roofRun: ', roofRun,

			',  miterType: ', miterType,

			',  holeStyle: ', holeStyle,

			',  vertPart: ', vertPart,

			',  thickness: ', thickness);

	END;

END;



BEGIN

	ForEachObject(ShowRoofFaceAttrib, ((SEL=TRUE)&amp;(T=71)));

END;

RUN(Example);
```

## Version
Availability: from VectorWorks9.0
## Category
* Objects - Roofs


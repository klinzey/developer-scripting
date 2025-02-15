# GetRoofAttributes

## Description
Function GetRoofAttributes returns the attributes of the referenced roof object.&lt;BR&gt;
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
&lt;/CENTER&gt;&lt;BR&gt;


```pascal
FUNCTION GetRoofAttributes(
				theRoof          : HANDLE;
				VAR genGableWall : BOOLEAN;
				VAR bearingInset : REAL;
				VAR roofThick    : REAL;
				VAR miterType    : INTEGER;
				VAR vertMiter    : REAL) : BOOLEAN;
```

```python

def vs.GetRoofAttributes(theRoof):
    return (BOOLEAN, genGableWall, bearingInset, roofThick, miterType, vertMiter)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theRoof|HANDLE|Handle to roof object.|
|genGableWall|BOOLEAN|Returns gable wall generation state.|
|bearingInset|REAL|Returns bearing inset dimension.|
|roofThick|REAL|Returns roof thickness.|
|miterType|INTEGER|Returns miter style.|
|vertMiter|REAL|Returns vertical miter dimension.|

## Remarks
genGableWall: Set to true to have a wall created at gable ends of the roof.  Otherwise no object will be inserted.<BR>
bearingInset  is where the weight of the roof rests on the wall.  This is an inset from the defining edge of the roof plan.<BR>
miterType: Specify 1 for a vertical miter, 2 for horizontal miter, 3 for a double miter cut, and 4 for a square end miter cut.<BR>
vertMiter: This is used only with the double miter type; it specifies the vertical length of the miter cut.

## Examples
```pascal
PROCEDURE Example;

var

	theRoof :HANDLE;

	genGableWall :BOOLEAN; 

	bearingInset, roofThick :REAL; 

	miterType :INTEGER; 

	vertMiter :REAL;

begin

	theRoof := FSActLayer;

	IF GetRoofAttributes(theRoof, genGableWall, bearingInset, roofThick, miterType, vertMiter)

	THEN Message(genGableWall, ' ', bearingInset, ' ', roofThick, ' ', miterType, ' ', vertMiter);

end;

RUN(Example);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


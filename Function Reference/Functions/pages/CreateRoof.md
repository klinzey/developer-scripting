# CreateRoof

## Description
Function CreateRoof creates a new roof object in a Vectorworks document, returning a handle to the object. To define the roof object template, use AppendRoofEdge.&lt;BR&gt;
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
FUNCTION CreateRoof(
				genGableWall         : BOOLEAN;
				bearingInsetDistance : REAL (Coordinate);
				roofThickDistance    : REAL (Coordinate);
				miterType            : INTEGER;
				vertMiterDistance    : REAL (Coordinate)) : HANDLE;
```

```python

def vs.CreateRoof(genGableWall, bearingInsetDistance, roofThickDistance, miterType, vertMiterDistance):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|genGableWall|BOOLEAN|Specifies gable roof generation.|
|bearingInsetDistance|REAL (Coordinate)|Bearing inset distance of wall into roof.|
|roofThickDistance|REAL (Coordinate)|Roof thickness.|
|miterType|INTEGER|Miter style of roof.|
|vertMiterDistance|REAL (Coordinate)|Vertical component for double miters.|

## Remarks
Use AppendRoofVertex() to define the roof plan.<BR>
genGableWall: Create wall object on gable ends, otherwise no wall is created.<BR>
bearingInset is where the weight of the roof rests on the wall.  This is an inset from the defining edge of the roof plan.<BR>
miterType:  1: vertical miter, 2: horizontal miter, 3: double miter , 4: square miter<BR>
vertMiter: Specifies vertical len of double miter.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,0&quot;);

AppendRoofEdge(roofHandle, -87'4&quot;,-38'4&quot;,#45d 0' 0&quot; ,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle, -30'2&quot;,-38'4&quot;,#45d 0' 0&quot; ,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle, -30'2&quot;,45'10&quot;,#45d 0' 0&quot; ,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle, -87'4&quot;,45'10&quot;,#45d 0' 0&quot; ,2'0&quot;,10'0&quot;);


```

## See Also
VS Functions:
[AppendRoofEdge](AppendRoofEdge.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


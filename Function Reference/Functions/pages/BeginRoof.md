# BeginRoof

## Description
Procedure BeginRoof creates a simple roof object in a Vectorworks document. &lt;BR&gt;
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
&lt;BR&gt;
&amp;lt;I&amp;gt;3-D View of Roof&amp;lt;/I&amp;gt;&amp;lt;P&amp;gt;&lt;BR&gt;
&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/roof.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;&lt;BR&gt;


```pascal
PROCEDURE BeginRoof(
				p1           : REAL;
				p2           : REAL;
				upslope      : REAL;
				riseDistance : REAL (Coordinate);
				runDistance  : REAL (Coordinate);
				miter        : INTEGER;
				vertPart     : REAL);
```

```python

def vs.BeginRoof(p1, p2, upslope, riseDistance, runDistance, miter, vertPart):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Coordinates of roof axis start point.|
|p2|REAL|Coordinates of roof axis end point.|
|upslope|REAL|Coordinates of upslope definition point.|
|riseDistance|REAL (Coordinate)|Rise distance.|
|runDistance|REAL (Coordinate)|Run distance.|
|miter|INTEGER|Edge miter style of roof.|
|vertPart|REAL|Dimension of vertical miter for double miter style.|

## Examples
```pascal
BeginRoof(1,1,5,1,2,2,0.5,1,1,0);

  ClosePoly;

  Poly(1,1,3,1,3.5,2,4,1,5,1,5,5,1,5);

EndGroup;




```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Roofs


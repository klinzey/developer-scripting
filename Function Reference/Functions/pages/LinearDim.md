# LinearDim

## Description
Procedure LinearDim creates a linear dimension in a Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
Bit code values for dimension flags can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#lindim&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;
&amp;lt;I&amp;gt;Linear Dimension&amp;lt;/I&amp;gt;&amp;lt;P&amp;gt;&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/lindim.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;

```pascal
PROCEDURE LinearDim(
				startPt        : REAL;
				endPt          : REAL;
				offsetDistance : REAL (Coordinate);
				dimType        : INTEGER;
				arrow          : INTEGER;
				textFlag       : INTEGER;
				textOffset     : REAL);
```

```python

def vs.LinearDim(startPt, endPt, offsetDistance, dimType, arrow, textFlag, textOffset):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startPt|REAL|X-Y coordinates of dimension start point.|
|endPt|REAL|X-Y coordinates of dimension end point.|
|offsetDistance|REAL (Coordinate)|Offset distance of dimension line from object.|
|dimType|INTEGER|Dimension type flag.|
|arrow|INTEGER|Arrowhead style flag.|
|textFlag|INTEGER|Text style flag.|
|textOffset|REAL|Dimension text offset distance.|

## Examples
```pascal
LinearDim(-2&quot;,2&quot;,1&quot;,2&quot;,-3&quot;,0,771,770,0.75);


```

## Version
Availability: from MiniCAD
## Category
* Dimensions


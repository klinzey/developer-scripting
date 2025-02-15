# CircularDim

## Description
Procedure CircularDim creates a diameter or radial dimension in a Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
Bit code values for dimension flags can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#lindim&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;
&amp;lt;I&amp;gt;Circular Dimension&amp;lt;/I&amp;gt;&amp;lt;P&amp;gt;&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/circdim.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;

```pascal
PROCEDURE CircularDim(
				startPt            : REAL;
				endPt              : REAL;
				box1               : REAL;
				box2               : REAL;
				textOffsetDistance : REAL (Coordinate);
				dimType            : INTEGER;
				arrow              : INTEGER;
				textFlag           : INTEGER;
				shoulder           : REAL);
```

```python

def vs.CircularDim(startPt, endPt, box1, box2, textOffsetDistance, dimType, arrow, textFlag, shoulder):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startPt|REAL|X-Y coordinates of dimension start point.|
|endPt|REAL|X-Y coordinates of dimension end point.|
|box1|REAL|X-Y coordinates of top left corner of object bounding box|
|box2|REAL|X-Y coordinates of bottom right corner of object bounding box|
|textOffsetDistance|REAL (Coordinate)|Offset distance of text from dimension line(witness leader length).|
|dimType|INTEGER|Dimension type flag.|
|arrow|INTEGER|Arrow style flag.|
|textFlag|INTEGER|Text style flag.|
|shoulder|REAL|Shoulder extension line length.|

## Examples
```pascal
CircularDim(-4 3/8&quot;,3&quot;,-4 3/8&quot;,1/4&quot;,-5 3/4&quot;,3&quot;,-3&quot;,1/4&quot;,1 1/8&quot;,1,3, 1025,1/4&quot;);




```

## Version
Availability: from MiniCAD
## Category
* Dimensions


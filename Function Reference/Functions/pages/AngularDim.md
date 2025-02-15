# AngularDim

## Description
Procedure AngularDim creates an angular dimension in the document.&lt;BR&gt;
&lt;BR&gt;
Bit code values for dimension flags can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#lindim&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;
&amp;lt;I&amp;gt;Angular Dimension&amp;lt;/I&amp;gt;&amp;lt;P&amp;gt;&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/angdim.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;

```pascal
PROCEDURE AngularDim(
				startPt            : REAL;
				endPt              : REAL;
				vert1              : REAL;
				textOffsetDistance : REAL (Coordinate);
				arrow              : INTEGER;
				textFlag           : INTEGER;
				posAngle           : REAL);
```

```python

def vs.AngularDim(startPt, endPt, vert1, textOffsetDistance, arrow, textFlag, posAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|startPt|REAL|X-Y coordinates of dimension start point.|
|endPt|REAL|X-Y coordinates of dimension end point|
|vert1|REAL|X-Y coordinates of dimension arc center.|
|textOffsetDistance|REAL (Coordinate)|Offset from dimension arc center (radius of the dimension arc).|
|arrow|INTEGER|Dimension arrowhead style flag.|
|textFlag|INTEGER|Dimension text style flag.|
|posAngle|REAL|Position angle of dimension text(from start). Auto position text overrides this value.|

## Examples
```pascal
AngularDim(1 1/2&quot;,3/8&quot;,-1/4&quot;,-1/2&quot;,7/8&quot;,-1/2&quot;,1.7001838&quot;,771,770,#35d 32'16&quot;);
```

## Version
Availability: from MiniCAD
## Category
* Dimensions


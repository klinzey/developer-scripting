# UnionRect

## Description
Procedure UnionRect returns a rectangle based on the boundary enclosing the two specified rectangles.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE UnionRect(
				p1     : REAL;
				p2     : REAL;
				p3     : REAL;
				p4     : REAL;
				VAR p5 : REAL;
				VAR p6 : REAL);
```

```python

def vs.UnionRect(p1, p2, p3, p4, p5, p6):
    return (p5, p6)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Top left coordinate of rectangle 1.|
|p2|REAL|Bottom right coordinate of rectangle 1.|
|p3|REAL|Top left coordinate of rectangle 2.|
|p4|REAL|Bottom right coordinate of rectangle 2.|
|p5|REAL|Top left coordinate of boundary rectangle.|
|p6|REAL|Bottom right coordinate of boundary rectangle.|

## Examples
```pascal
UnionRect(0,0,3,3,3,3,5,5,x1,y1,x2,y2);
```

## Version
Availability: from MiniCAD
## Category
* Graphic Calculation


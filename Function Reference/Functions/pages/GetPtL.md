# GetPtL

## Description
Procedure GetPtL creates a temporary &amp;quot;rubberband&amp;quot; line from a specified point to the user selected end point. This cannot be used if there is a function anywhere in the calling chain.

```pascal
PROCEDURE GetPtL(
				p1     : REAL;
				VAR p2 : REAL);
```

```python

def vs.GetPtL(p1):
    return p2
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Coordinates of line start point.|
|p2|REAL|Returns coordinates of mouse click.|

## Examples
```pascal
PROCEDURE Example;

VAR

	pt1, pt2 :VECTOR;

BEGIN

	GetPt(pt1.x, pt1.y);

	GetPtL(pt1.x, pt1.y, pt2.x, pt2.y);

	MoveTo(pt1.x, pt1.y);

	LineTo(pt2.x, pt2.y);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* User Interactive


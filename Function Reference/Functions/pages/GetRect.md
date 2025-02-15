# GetRect

## Description
Procedure GetRect draws a temporary &amp;quot;rubberband&amp;quot; rectangle onscreen, similar to a selection marquee. The user defines the rectangle by selecting two points which define the top left and bottom right of the rectangle. This cannot be used if there is a function anywhere in the calling chain.

```pascal
PROCEDURE GetRect(
				VAR p1 : REAL;
				VAR p2 : REAL);
```

```python

def vs.GetRect():
    return (p1, p2)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Returns coordinates of first user click.|
|p2|REAL|Returns coordinates of second user click.|

## Version
Availability: from MiniCAD
## Category
* User Interactive


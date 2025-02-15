# GetLine

## Description
Procedure GetLine returns two user selected points, and draws a temporary &amp;quot;rubberband&amp;quot; line when prompting for the second point. This cannot be used if there is a function anywhere in the calling chain.

```pascal
PROCEDURE GetLine(
				VAR p1 : REAL;
				VAR p2 : REAL);
```

```python

def vs.GetLine():
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


# LineEllipseIntersect

## Description
Calculates the intersection between the specified line and ellipse.

```pascal
PROCEDURE LineEllipseIntersect(
				a1         : REAL;
				a2         : REAL;
				upperRight : REAL;
				lowerLeft  : REAL;
				VAR int1   : REAL;
				VAR legal1 : BOOLEAN;
				VAR int2   : REAL;
				VAR legal2 : BOOLEAN);
```

```python

def vs.LineEllipseIntersect(a1, a2, upperRight, lowerLeft):
    return (int1, legal1, int2, legal2)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|a1|REAL|Start point of the line|
|a2|REAL|End point of the line|
|upperRight|REAL|Upper-right point of the ellipse|
|lowerLeft|REAL|Lower-left point of the ellipse|
|int1|REAL|On return, first point of intersection, if found|
|legal1|BOOLEAN|On return, second point of intersection, if found|
|int2|REAL|On return, indicates that int1 is a valid point of intersection|
|legal2|BOOLEAN|On return, indicates that int2 is a valid point of intersection|

## Remarks
On return, int1 and int2 are the two possible points of intersection.  legal1 and legal2 indicate if the intersections are actually valid.

## Version
Availability: from VectorWorks10.0
## Category
* Graphic Calculation


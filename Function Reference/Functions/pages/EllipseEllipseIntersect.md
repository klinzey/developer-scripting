# EllipseEllipseIntersect

## Description
Calculates the intersections between the two specified ellipses.

```pascal
FUNCTION EllipseEllipseIntersect(
				upperLeft1  : REAL;
				lowerRight1 : REAL;
				upperLeft2  : REAL;
				lowerRight2 : REAL;
				VAR int1    : REAL;
				VAR int2    : REAL;
				VAR int3    : REAL;
				VAR int4    : REAL) : INTEGER;
```

```python

def vs.EllipseEllipseIntersect(upperLeft1, lowerRight1, upperLeft2, lowerRight2):
    return (INTEGER, int1, int2, int3, int4)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|upperLeft1|REAL|Upper-left point of the first ellipse|
|lowerRight1|REAL|Lower-right point of the first ellipse|
|upperLeft2|REAL|Upper-left point of the second ellipse|
|lowerRight2|REAL|Lower-right point of the second ellipse|
|int1|REAL|On return, first point of intersection, if found|
|int2|REAL|On return, second point of intersection, if found|
|int3|REAL|On return, third point of intersection, if found|
|int4|REAL|On return, fourth point of intersection, if found|

## Returns
Returns the number of valid intersection points.  If the return value is n, the first n points are valid.  For example, if the return value is 1, the int1 parameter contains a valid point of intersection, and int2, int3, and int4 are invalid.  If the return value is 3, int1, int2, and int3 contain valid points, and int4 is invalid.

## Remarks
On return, int1, int2, int3, and int4 contain the points of intersection.  Return value indicates which intersections are legal.

## Examples
```pascal
PROCEDURE Example;

VAR

	h1, h2 :HANDLE;

	upperLeft1, lowerRight1 :POINT;

	upperLeft2, lowerRight2 :POINT;

	int1, int2, int3, int4 :POINT;

	num :INTEGER;

BEGIN

	CallTool(-205); h1 := FSActLayer;

	CallTool(-205); h2 := FSActLayer;

	GetBBox(h1, upperLeft1.x, upperLeft1.y, lowerRight1.x, lowerRight1.y);

	GetBBox(h2, upperLeft2.x, upperLeft2.y, lowerRight2.x, lowerRight2.y);

	num := EllipseEllipseIntersect(upperLeft1, lowerRight1, upperLeft2, lowerRight2, int1, int2, int3, int4);

	Message(num);

	Locus(int1.x, int1.y);

	Locus(int2.x, int2.y);

	Locus(int3.x, int3.y);

	Locus(int4.x, int4.y);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks10.0
## Category
* Graphic Calculation


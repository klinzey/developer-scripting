# AngBVec

## Description
Returns the positive angle between the two specified vectors, in the range of 0~180 degrees.&lt;BR&gt;
&lt;BR&gt;
When used with 3D vectors, the angle returned will be in a plane defined by the two vectors.

```pascal
FUNCTION AngBVec(
				v1 : VECTOR;
				v2 : VECTOR) : REAL;
```

```python

def vs.AngBVec(v1, v2):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v1|VECTOR|First vector to be compared.|
|v2|VECTOR|Second vector to be compared.|

## Returns
Returns a REAL value which is the angle (in degrees) between the two vectors.

## Examples
```pascal
PROCEDURE Example;

VAR

	pt1, pt2, pt3, pt4 :VECTOR;

BEGIN

	GetPt(pt1.x, pt1.y);

	GetPtL(pt1.x, pt1.y, pt2.x, pt2.y);

	GetPtL(pt2.x, pt2.y, pt3.x, pt3.y);

	MoveTo(pt1.x, pt1.y);

	LineTo(pt2.x, pt2.y);

	LineTo(pt3.x, pt3.y);

	pt4 := (pt1 + pt3) / 2;

	TextOrigin(pt4.x, pt4.y);

	CreateText(Concat(AngBVec(pt1 - pt2, pt3 - pt2)));

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Math - Vectors


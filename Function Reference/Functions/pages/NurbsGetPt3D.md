# NurbsGetPt3D

## Description
Returns the coordinates of a point in the referenced NURBS curve or surface.&lt;BR&gt;
&lt;BR&gt;
The index is zero based (0 to number of points - 1).

```pascal
PROCEDURE NurbsGetPt3D(
				objectHd : HANDLE;
				index1   : LONGINT;
				index2   : LONGINT;
				VAR p    : REAL);
```

```python

def vs.NurbsGetPt3D(objectHd, index1, index2):
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to NURBS curve or surface.|
|index1|LONGINT|Index of point in NURBS curve, or u-coordinate of point location in NURBS surface.|
|index2|LONGINT|V-coordinate of point location in NURBS surface.|
|p|REAL|Coordinates of the control point.|

## Remarks
this function will work for both nurbs curves and nurbs surfaces. <BR>
<BR>
Gets the index2 vertex of the indexe1 piece of the given NURBS curve or the index1 U and index2 V control point of the surfaces.

## See Also
VS Functions:
[NurbsCurveEvalPt](NurbsCurveEvalPt.md)| [NurbsSurfaceEvalPt](NurbsSurfaceEvalPt.md)

## Version
Availability: from VectorWorks9.0
## Category
* Objects - NURBS


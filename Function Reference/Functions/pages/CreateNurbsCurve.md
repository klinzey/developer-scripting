# CreateNurbsCurve

## Description
Creates a new NURBS curve in the document. 

```pascal
FUNCTION CreateNurbsCurve(
				first     : REAL;
				byCtrlPts : BOOLEAN;
				degree    : INTEGER) : HANDLE;
```

```python

def vs.CreateNurbsCurve(first, byCtrlPts, degree):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|first|REAL|Coordinates of the first point in the curve definiton.|
|byCtrlPts|BOOLEAN|Create curve by control points (not interpolation).|
|degree|INTEGER|The degree of the NURBS curve.|

## Returns
Returns a HANDLE to the new NURBS curve if successful, otherwise returns NIL.

## Remarks
CreateNurbsCurve returns a handle to the newly created NURBS curve, if successful<BR>
<BR>
Creates a NURBS curve with a single fit or control point , if it succeeds, return nil if it fails

## Examples
```pascal
PROCEDURE NewNurbsCurve;

VAR

	nC :HANDLE;

BEGIN

	nC := CreateNurbsCurve(0, 0, 0, true, 2);

	AddVertex3D(nC, 1, 1, 0);

	AddVertex3D(nC, 2, 0, 0);

END;

RUN(NewNurbsCurve);


```

## Version
Availability: from VectorWorks9.0
## Category
* Objects - NURBS


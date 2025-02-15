# GetRoofFaceCoords

## Description
Returns the coordinates of the defining geometry of a roof face.

```pascal
PROCEDURE GetRoofFaceCoords(
				h           : HANDLE;
				VAR axis1   : REAL;
				VAR axis2   : REAL;
				VAR Zaxis   : REAL;
				VAR upslope : REAL);
```

```python

def vs.GetRoofFaceCoords(h):
    return (axis1, axis2, Zaxis, upslope)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to roof face object.|
|axis1|REAL|X-Y coordinates of first axis point.|
|axis2|REAL|X-Y coordinates of second axis point.|
|Zaxis|REAL|Elevation of roof axis.|
|upslope|REAL|X-Y coordinates of roof upslope point.|

## Remarks
Returns information about old-style roof objects (single roof faces).<BR>
<BR>
Returns roof definition axis, upslope definition point.<BR>
<BR>
See Also GetRoofFaceAttr() for additional roof face data

## Examples
```pascal
PROCEDURE GetRoofFaceCoordsExample;



PROCEDURE MarkCoords(h :HANDLE);

VAR

	beg_pt, end_pt, upslope_pt :VECTOR;

	Z :REAL;

BEGIN

	IF GetObjectVariableInt(h, 172) = 1 THEN BEGIN

		GetRoofFaceCoords(h, beg_pt.x, beg_pt.y, end_pt.x, end_pt.y, Z, upslope_pt.x, upslope_pt.y);

		beg_pt     := beg_pt     * (25.4 / GetPrefReal(152));

		end_pt     := end_pt     * (25.4 / GetPrefReal(152));

		upslope_pt := upslope_pt * (25.4 / GetPrefReal(152));

		Locus(beg_pt.x, beg_pt.y);

		Locus(end_pt.x, end_pt.y);

		Locus(upslope_pt.x, upslope_pt.y);

	END;

END;



BEGIN

	ForEachObject(MarkCoords, (T=71));

END;

RUN(GetRoofFaceCoordsExample);
```

## Version
Availability: from VectorWorks9.0
## Category
* Objects - Roofs


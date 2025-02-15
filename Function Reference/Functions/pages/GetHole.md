# GetHole

## Description
Returns a handle to a polyline defining an opening within the referenced polyline.&lt;BR&gt;
&lt;BR&gt;
The definition polyline can be edited or queried using the standard VectorScript polyline API functions.

```pascal
FUNCTION GetHole(
				inOutsidePolyline : HANDLE;
				inIndex           : INTEGER;
				VAR outHole       : HANDLE) : BOOLEAN;
```

```python

def vs.GetHole(inOutsidePolyline, inIndex):
    return (BOOLEAN, outHole)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inOutsidePolyline|HANDLE|Handle to polyline.|
|inIndex|INTEGER|Index number of opening definition polyline.|
|outHole|HANDLE|Handle to definition polyline.|

## Returns
Returns TRUE if the polyline contains openings, otherwise returns FALSE.

## Examples
```pascal
PROCEDURE Example;

VAR

	inPolyline  :HANDLE;

	outNumHoles :INTEGER;

	inIndex     :INTEGER;

	outHole     :HANDLE;

	vertexNum   :INTEGER;

	pX, pY      :REAL;

	vertexType  :INTEGER;

	arcRadius   :REAL;

BEGIN

	inPolyline := FSActLayer;

	IF GetNumHoles(inPolyline, outNumHoles) THEN BEGIN

		FOR inIndex := 1 TO outNumHoles DO BEGIN

			if GetHole(inPolyline, inIndex, outHole) THEN BEGIN

				FOR vertexNum := 1 TO GetVertNum(outHole) DO BEGIN

					GetPolylineVertex(outHole, vertexNum, pX, pY, vertexType, arcRadius);

					WriteLn('pX: ', pX, ' pY: ', pY);

				END;

			END;

		END;

	END;

END;

RUN(Example);


```

## See Also
VS Functions:
[GetNumHoles](GetNumHoles.md)

## Version
Availability: from VectorWorks9.0
## Category
* Objects - Polys


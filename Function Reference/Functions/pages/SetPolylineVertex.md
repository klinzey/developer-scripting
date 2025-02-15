# SetPolylineVertex

## Description
Sets the attributes of the specified polyline vertex to the specified values.

```pascal
PROCEDURE SetPolylineVertex(
				obj               : HANDLE;
				vertexNum         : INTEGER;
				p                 : REAL;
				vertexType        : INTEGER;
				arcRadiusDistance : REAL (Coordinate);
				recalcBounds      : BOOLEAN);
```

```python

def vs.SetPolylineVertex(obj, vertexNum, p, vertexType, arcRadiusDistance, recalcBounds):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|vertexNum|INTEGER|Index (1-based) of vertex to be modified.|
|p|REAL|New X-Y coordinates of vertex.|
|vertexType|INTEGER|Type of vertex.|
|arcRadiusDistance|REAL (Coordinate)|Radius of vertex corner (arc vertex only).|
|recalcBounds|BOOLEAN|Recalculate object bounds.|

## Remarks
Sets the specified vertex of the referenced polyline object.  Vertex type constant values are 0 - Corner, 1 - Bezier, 2 - Cubic, 3 - Arc

## Examples
```pascal
PROCEDURE Example;

   {This will convert anything it can in the drawing to a polyline

   (including rectangles, polygons, etc.), and then it will fillet

   all of the corners with a radius of .015&quot;.}

CONST

   kFilletRadius = .015&quot;;

VAR

   cnt :INTEGER;

   x, y :REAL;

   vertexType :INTEGER;

   vertexRadius :REAL;

   criteria :STRING;



PROCEDURE FilletPolygon(h :HANDLE);

BEGIN

   h := ConvertToPolyline(h);

   FOR cnt := 1 to GetVertNum(h) DO BEGIN

      GetPolylineVertex(h, cnt, x, y, vertexType, vertexRadius);

      SetPolylineVertex(h, cnt, x, y, 3, kFilletRadius, TRUE);

   END;

END;



BEGIN

   criteria := '(ALL)';

   ForEachObject(FilletPolygon, criteria);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Polys


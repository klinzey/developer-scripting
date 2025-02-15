# ArcTo

## Description
Procedure ArcTo creates an arc vertex with a point of intersection at the specified coordinate point.&lt;BR&gt;
&lt;BR&gt;
The endpoints of the arc are tangent to the control segments which intersect at p. If a radius of 0 is passed as the parameter, the arc endpoints will be at the vertices preceding and following the arc spline vertex.

```pascal
PROCEDURE ArcTo(
				p              : REAL;
				radiusDistance : REAL (Coordinate));
```

```python

def vs.ArcTo(p, radiusDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Coordinates of vertex.|
|radiusDistance|REAL (Coordinate)|Radius of vertex arc.|

## Examples
```pascal
BeginPoly;

   LineTo(-1&quot;,2&quot;);

   LineTo(-2 1/2&quot;,1/2&quot;);

   CurveTo(-1 1/2&quot;,-1 1/2&quot;);

   LineTo(1&quot;,-1/2&quot;);

   ArcTo(1&quot;,1 1/2&quot;,1/2&quot;);

EndPoly;

{creates a polyline object}
```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Polys


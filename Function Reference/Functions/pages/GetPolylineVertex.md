# GetPolylineVertex

## Description
Returns information about the specified polyline vertex.&lt;BR&gt;
&lt;BR&gt;
Note that vertexNum is 1-based for Polygons and Polylines, and 0-based for 3D Polylines.

```pascal
PROCEDURE GetPolylineVertex(
				obj            : HANDLE;
				vertexNum      : INTEGER;
				VAR p          : REAL;
				VAR vertexType : INTEGER;
				VAR arcRadius  : REAL);
```

```python

def vs.GetPolylineVertex(obj, vertexNum):
    return (p, vertexType, arcRadius)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|vertexNum|INTEGER|Index of vertex to be queried. |
|p|REAL|X-Y coordinates of vertex.|
|vertexType|INTEGER|Type of vertex.|
|arcRadius|REAL|Radius of vertex corner (arc vertex only).|

## Remarks
Retrieves information about a polyline vertex.  Vertex type constant values are 0 - Corner, 1 - Bezier, 2 - Cubic, 3 - Arc

## Examples
```pascal
PROCEDURE Example;

VAR

	obj        :HANDLE;

	vertexNum  :INTEGER;

	ptX, ptY   :REAL;

	vertexType :INTEGER;

	arcRadius  :REAL;

BEGIN

	obj := FSActLayer;

	FOR vertexNum := 1 TO GetVertNum(obj) DO BEGIN

		GetPolylineVertex(obj, vertexNum, ptX, ptY, vertexType, arcRadius);

		TextOrigin(ptX, ptY);

		CreateText(Concat('vNum: ', vertexNum, '  vType: ', vertexType, '  radius: ', arcRadius));

	END;

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Polys


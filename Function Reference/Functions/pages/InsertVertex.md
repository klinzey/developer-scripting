# InsertVertex

## Description
Inserts a new vertex into polygon or polyline.  If the vertexType is nonzero, it will convert the objectHandle into a polyline.

```pascal
PROCEDURE InsertVertex(
				objectHandle    : HANDLE;
				x               : REAL;
				y               : REAL;
				beforeVertexNum : INTEGER;
				vertexType      : INTEGER;
				arcRadius       : REAL);
```

```python

def vs.InsertVertex(objectHandle, x, y, beforeVertexNum, vertexType, arcRadius):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to the polygon or polyline|
|x|REAL|X-coordinate of the vertex to add|
|y|REAL|Y-coordinate of the vertex to add|
|beforeVertexNum|INTEGER|Vertex number before which the new vertex is to be inserted|
|vertexType|INTEGER|Vertex type of the new vertex|
|arcRadius|REAL|For arc vertices, the radius of the arc|

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Polys


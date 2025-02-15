# Add2DVertex

## Description
This procedure will add to a polyline a vertex defined by its position, its type(0 to 4) and the radius if type is 3 or 4. A vertex of type 4 should be followed and preceded by corner vertices. If the type is equal to 4, the point will be a middle point of an arc. In this case if the radius is not given (0) it will be computed.

```pascal
PROCEDURE Add2DVertex(
				p          : REAL;
				vertexType : INTEGER;
				arcRadius  : REAL (Coordinate));
```

```python

def vs.Add2DVertex(p, vertexType, arcRadius):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|The vertex to add to a polyline.|
|vertexType|INTEGER|The type of the vertex it could be 0, 1, 2, 3 or 4.|
|arcRadius|REAL (Coordinate)|The arc radius if the vertex type is 3 or 4.|

## Examples
```pascal
beginPoly;

Add2DVertex(0,0,0,0);

Add2DVertex(1,1,4,0);

Add2DVertex(2,0,0,0);

Add2DVertex(3,1,4,0);

Add2DVertex(4,0,0,0);

endPoly;
```

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Polys


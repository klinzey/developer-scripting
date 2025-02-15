# SetRoofEdge

## Description
Procedure SetRoofEdge sets the definition attributes of a roof edge for the referenced roof object.

```pascal
PROCEDURE SetRoofEdge(
				roofObject         : HANDLE;
				index              : INTEGER;
				vertexPt           : REAL;
				edgeAngle          : REAL;
				projectionDistance : REAL (Coordinate);
				eaveHeightDistance : REAL (Coordinate));
```

```python

def vs.SetRoofEdge(roofObject, index, vertexPt, edgeAngle, projectionDistance, eaveHeightDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|index|INTEGER|Index of roof edge.|
|vertexPt|REAL|Coordinates of roof edge vertex.|
|edgeAngle|REAL|Roof slope.|
|projectionDistance|REAL (Coordinate)|Eave overhang.|
|eaveHeightDistance|REAL (Coordinate)|Eave height.|

## Remarks
Vertices define the outline of the roof and its characteristics.  Vertices must progress in a counter clock wise direction, when viewed from a top view, otherwise the roof cannot be built.<BR>
<BR>
index: Indexs have values between 1 and NVertices (See GetRoofVertices())<BR>
edgePt: Coordinate point for this edge<BR>
slope: pitch of this roof edge<BR>
projection: eave overhang<BR>
eaveHeight: eave height

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


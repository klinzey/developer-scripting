# AppendRoofEdge

## Description
Function AppendRoofEdge creates a new edge in the referenced roof object.

```pascal
PROCEDURE AppendRoofEdge(
				theRoof            : HANDLE;
				edgePt             : REAL;
				slopeAngle         : REAL;
				projectionDistance : REAL (Coordinate);
				eaveHeightDistance : REAL (Coordinate));
```

```python

def vs.AppendRoofEdge(theRoof, edgePt, slopeAngle, projectionDistance, eaveHeightDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theRoof|HANDLE|Handle to roof.|
|edgePt|REAL|Definition point of roof edge.|
|slopeAngle|REAL|Slope of roof edge.|
|projectionDistance|REAL (Coordinate)|Eave overhang.|
|eaveHeightDistance|REAL (Coordinate)|Eave height.|

## Remarks
Vertex is appended to the end of the list of vertices.  Vertices define the outline of the roof.  Vertices must progress in a counter clock wise direction, when viewed from a top view, otherwise the roof cannot be built.<BR>
<BR>
edgePt: Coordinate point for this edge<BR>
slope: pitch of this roof edge<BR>
projection: eave overhang<BR>
eaveHeight: eave height

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45d0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45d0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45d0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,21'4.81922&quot;,#45d0'0&quot;,2'0&quot;,10'0&quot;);

shedID := CreateShedDormer(roofHandle);

SetShedAttributes(roofHandle,shedID,TRUE,6'0&quot;,10'0&quot;,2'0&quot;,#8d0'0&quot;);

SetDormerAttributes(roofHandle, shedID, 3,18'4&quot;,TRUE,3'0&quot;,63,FALSE,3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


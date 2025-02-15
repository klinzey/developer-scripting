# SetBatAttributes

## Description
Procedure SetBatAttributes sets the attributes of a bat dormer in the referenced roof. 

```pascal
PROCEDURE SetBatAttributes(
				roofObject               : HANDLE;
				dormerID                 : INTEGER;
				useHeight                : BOOLEAN;
				heightDepthValueDistance : REAL (Coordinate);
				bottomWidthDistance      : REAL (Coordinate);
				topWidthDistance         : REAL (Coordinate);
				baseHeightDistance       : REAL (Coordinate);
				controlPointDistance     : REAL (Coordinate);
				topAngle                 : REAL);
```

```python

def vs.SetBatAttributes(roofObject, dormerID, useHeight, heightDepthValueDistance, bottomWidthDistance, topWidthDistance, baseHeightDistance, controlPointDistance, topAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|dormerID|INTEGER|Index of dormer element.|
|useHeight|BOOLEAN|Use height setting to create dormer element.|
|heightDepthValueDistance|REAL (Coordinate)|Height/depth distance.|
|bottomWidthDistance|REAL (Coordinate)|Bottom width.|
|topWidthDistance|REAL (Coordinate)|Top width.|
|baseHeightDistance|REAL (Coordinate)|Base height of bat.|
|controlPointDistance|REAL (Coordinate)|Offset distance of control point.|
|topAngle|REAL|Slope of bat roof.|

## Remarks
dormerID: Identifies the dormer for which to set the information.<BR>
<BR>
useHeight: Set to true if the next value is the height of the dormer, if false, next value is the depth (front to back) of the dormer.<BR>
heightDepthValue: Size of the dormer, either by height or depth; determined by previous parameter.<BR>
<BR>
bottomWidth: Dimension of bottom front edge of the dormer, left to right..<BR>
topWidth: Dimension of the roof of the dormer.<BR>
baseHeight: Dimension of the bottom half of the dormer.<BR>
<BR>
topSlope: Angle of the dormer roof.<BR>
<BR>
controlPoint: The distance from the side to where the curve starts.  Must be less than (bottomWidth - topWidth) / 2.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

batID := CreateBatDormer(roofHandle);

SetBatAttributes(roofHandle,batID,TRUE,5'0&quot;,10'0&quot;,4'0&quot;,6'3&quot;,2'0&quot;,#8°0'0&quot;);

SetDormerAttributes(roofHandle,batID,3,18'4&quot;,TRUE,3'0&quot;,63,FALSE,3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


# SetHipAttributes

## Description
Procedure SetHipAttributes sets the attributes of a hip dormer in the referenced roof. 

```pascal
PROCEDURE SetHipAttributes(
				roofObject          : HANDLE;
				dormerID            : INTEGER;
				useHeight           : BOOLEAN;
				heightDepthDistance : REAL (Coordinate);
				bottomWidthDistance : REAL (Coordinate);
				overhangDistance    : REAL (Coordinate);
				leftAngle           : REAL;
				rightAngle          : REAL;
				frontAngle          : REAL);
```

```python

def vs.SetHipAttributes(roofObject, dormerID, useHeight, heightDepthDistance, bottomWidthDistance, overhangDistance, leftAngle, rightAngle, frontAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|dormerID|INTEGER|Index of dormer element.|
|useHeight|BOOLEAN|Use height setting to create dormer element.|
|heightDepthDistance|REAL (Coordinate)|Height/depth distance.|
|bottomWidthDistance|REAL (Coordinate)|Bottom width.|
|overhangDistance|REAL (Coordinate)|Overhang distance.|
|leftAngle|REAL|Slope of left roof of dormer.|
|rightAngle|REAL|Slope of right roof of dormer.|
|frontAngle|REAL|Slope of front roof of dormer.|

## Remarks
dormerID: Identifies the dormer for which to set the information.<BR>
<BR>
useHeight: Set to true if the next value is the height of the dormer, if false, next value is the depth (front to back) of the dormer.<BR>
heightDepthValue: Size of the dormer, either by height or depth; determined by previous parameter.<BR>
<BR>
bottomWidth: Dimension of bottom front edge of the dormer, left to right.<BR>
<BR>
leftSlope: Angle of left dormer roof.<BR>
rightSlope: Angle of right dormer roof.<BR>
frontSlope: Angle of the front dormer roof face.<BR>
<BR>
overhang: Distance roof projects past dormer walls.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

hipID := CreateHipDormer(roofHandle);

SetHipAttributes(roofHandle, hipID,TRUE,6'0&quot;,10'0&quot;,2'0&quot;,#45°0'0&quot;,#45°0'0&quot;,#45°0'0&quot;);

SetDormerAttributes(roofHandle, hipID, 3,18'4&quot;,TRUE,3'0&quot;,63,FALSE,3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


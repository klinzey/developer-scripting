# SetShedAttributes

## Description
Procedure SetShedAttributes sets the attributes of a shed dormer in the referenced roof. 

```pascal
PROCEDURE SetShedAttributes(
				roofObject          : HANDLE;
				dormerID            : INTEGER;
				useHeight           : BOOLEAN;
				heightDepthDistance : REAL (Coordinate);
				bottomWidthDistance : REAL (Coordinate);
				overhangDistance    : REAL (Coordinate);
				topAngle            : REAL);
```

```python

def vs.SetShedAttributes(roofObject, dormerID, useHeight, heightDepthDistance, bottomWidthDistance, overhangDistance, topAngle):
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
|topAngle|REAL|Top angle of dormer element.|

## Remarks
dormerID: Identifies the dormer for which to set the information.<BR>
<BR>
useHeight: true if the next value is the height of the dormer, if false, next value is the depth (front to back) of the dormer<BR>
heightDepthValue: size of the dormer, either by height or depth; determined by previous parameter.<BR>
<BR>
bottomWidth: Dimension of bottom front edge of the dormer, left to right.<BR>
<BR>
topSlope: Angle of dormer roof.<BR>
<BR>
overhang: Distance roof projects past dormer walls.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,21'4.81922&quot;,#45°0'0&quot; ,2'0&quot;,10'0&quot;);

shedID := CreateShedDormer(roofHandle);

SetShedAttributes(roofHandle,shedID,TRUE,6'0&quot;,10'0&quot;,2'0&quot;,#8°0'0&quot;);

SetDormerAttributes(roofHandle,shedID,3,18'4&quot;,TRUE,3'0&quot;,63,FALSE, 3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


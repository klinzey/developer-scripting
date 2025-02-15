# SetTrapeziumAttributes

## Description
Procedure SetTrapeziumAttributes sets the attributes of a trapezium dormer in the referenced roof. 

```pascal
PROCEDURE SetTrapeziumAttributes(
				roofObject          : HANDLE;
				dormerID            : INTEGER;
				useHeight           : BOOLEAN;
				heightDpthDistance  : REAL (Coordinate);
				bottomWidthDistance : REAL (Coordinate);
				useTopWidth         : BOOLEAN;
				topWidthDistance    : REAL (Coordinate);
				leftAngle           : REAL;
				rightAngle          : REAL;
				topAngle            : REAL);
```

```python

def vs.SetTrapeziumAttributes(roofObject, dormerID, useHeight, heightDpthDistance, bottomWidthDistance, useTopWidth, topWidthDistance, leftAngle, rightAngle, topAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|dormerID|INTEGER|Index of dormer element.|
|useHeight|BOOLEAN|Use height setting to create dormer element.|
|heightDpthDistance|REAL (Coordinate)|Height/depth distance.|
|bottomWidthDistance|REAL (Coordinate)|Bottom width.|
|useTopWidth|BOOLEAN|Use top width to create dormer element.|
|topWidthDistance|REAL (Coordinate)|Top width.|
|leftAngle|REAL|Left roof slope.|
|rightAngle|REAL|Right roof slope.|
|topAngle|REAL|Top roof slope.|

## Remarks
dormerID: Identifies the which dormer for which to set the values.<BR>
<BR>
useHeight: Set to true if the next value is the height of the dormer, otherwise set to false if the next value is the depth (front to back) of the dormer.<BR>
heightDepthValue: Size of the dormer, either by height or depth; determined by previous parameter.<BR>
<BR>
bottomWidth: Dimension of bottom front edge of the dormer, left to right.<BR>
<BR>
useTopWidth: True if using a dimension to set the width of the dormer roof.  False if the top width of the dormer is determined by the left and right slope.  The topWidth is exclusive of leftSlope &amp; rightSlope.<BR>
twOrLSlope: dimension of the roof of the dormer if previous param is true, or slope of left dormer wall if false.<BR>
rightSlope: Angle of right dormer wall.<BR>
<BR>
topSlope: Angle of the roof of the dormer.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle, -77'10&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

trapID:=CreateTrapeziumDormer(roofHandle);

SetTrapeziumAttributes(roofHandle,trapID,TRUE,6'0&quot;,10'0&quot;,TRUE,6'0&quot;,#0°0'0&quot;,#0°0'0&quot;,#8°0'0&quot;);

SetDormerAttributes(roofHandle,trapID,3,18'4&quot;,TRUE,3'0&quot;,63,FALSE,3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


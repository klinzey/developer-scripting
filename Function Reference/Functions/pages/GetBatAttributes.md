# GetBatAttributes

## Description
Procedure GetBatAttributes returns the attributes of a bat dormer in the referenced roof. 

```pascal
PROCEDURE GetBatAttributes(
				roofObject       : HANDLE;
				dormerID         : INTEGER;
				VAR useHeight    : BOOLEAN;
				VAR heightDepth  : REAL;
				VAR bottomWidth  : REAL;
				VAR topWidth     : REAL;
				VAR baseHeight   : REAL;
				VAR controlPoint : REAL;
				VAR topSlope     : REAL);
```

```python

def vs.GetBatAttributes(roofObject, dormerID):
    return (useHeight, heightDepth, bottomWidth, topWidth, baseHeight, controlPoint, topSlope)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|dormerID|INTEGER|Index of dormer element.|
|useHeight|BOOLEAN|Returns if height setting was used to created dormer.|
|heightDepth|REAL|Returns height or depth value.|
|bottomWidth|REAL|Returns bottom width.|
|topWidth|REAL|Returns top width.|
|baseHeight|REAL|Returns base height.|
|controlPoint|REAL|Returns the control point offset.|
|topSlope|REAL|Returns the slope of the bat roof.|

## Remarks
This will fail if the dormerID identifies a dormer of a different style, or the dormerID is not valid.<BR>
<BR>
dormerID: Identifies the dormer for which to retrieve the information.<BR>
<BR>
useHeight: Set to true if the next value is the height of the dormer, if false, next value is the depth (front to back) of the dormer.<BR>
heightDepthValue: Size of the dormer, either by height or depth; determined by previous parameter.<BR>
<BR>
bottomWidth: Dimension of bottom front edge of the dormer, left to right.<BR>
baseHeight: Dimension of the bottom half of the dormer.<BR>
topWidth: Dimension of the roof of the dormer.<BR>
<BR>
topSlope: Angle of the dormer roof.<BR>
<BR>
controlPoint: The distance from the side to where the curve starts.  Must be less than (bottomWidth - topWidth) / 2.

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


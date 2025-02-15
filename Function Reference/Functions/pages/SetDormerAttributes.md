# SetDormerAttributes

## Description
Procedure SetDormerAttributes sets the attributes of a roof element in the referenced roof. 

```pascal
PROCEDURE SetDormerAttributes(
				roofObject                 : HANDLE;
				dormerID                   : INTEGER;
				edgeIndex                  : INTEGER;
				cornerOffsetDistance       : REAL (Coordinate);
				isPerpOffset               : BOOLEAN;
				perpOrHeightOffsetDistance : REAL (Coordinate);
				symName                    : LONGINT;
				centerSymbol               : BOOLEAN;
				symOffsetDistance          : REAL (Coordinate));
```

```python

def vs.SetDormerAttributes(roofObject, dormerID, edgeIndex, cornerOffsetDistance, isPerpOffset, perpOrHeightOffsetDistance, symName, centerSymbol, symOffsetDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|dormerID|INTEGER|Index of dormer element.|
|edgeIndex|INTEGER|Index of roof edge.|
|cornerOffsetDistance|REAL (Coordinate)|Corner offset distance.|
|isPerpOffset|BOOLEAN|Specifies perpendicular or height offset.|
|perpOrHeightOffsetDistance|REAL (Coordinate)|Perpendicular or height offset distance.|
|symName|LONGINT|Index of dormer symbol.|
|centerSymbol|BOOLEAN|Specifies if symbol is centered.|
|symOffsetDistance|REAL (Coordinate)|Symbol offset distance.|

## Remarks
This will fail if the dormerID identifies a skylight, or dormerID is not valid.<BR>
<BR>
dormerID: Identifies the dormer for which to set the information.<BR>
edgeIndex: Index to which roof face this dormer is placed.  Value is one based.<BR>
<BR>
cornerOffset: Distance from the vertex to the center of the dormer.<BR>
isPerpOffset: Determines the meaning of the next parameter.  Set to true for the value to be the plan distance from the outline to the front of the dormer.  Set to false for offsetValue to set the distance from the top of the dormer to the bearing height.<BR>
perpOrHeightOffset: Either the distance from the outline to the front of the dormer, or from the dormer roof to the floor.<BR>
<BR>
symName: Symbol to place in the dormer, this is the window.<BR>
centerSymbol: Set to true to vertically center the symbol in the dormer.  Doing so causes the next parameter to be ignored.<BR>
Set to false to offset the symbol from the top of the dormer using the next parameter.<BR>
symOffset: Distance from top of the dormer to symbol insertion point.

## Examples
```pascal
roofHandle := CreateRoof(TRUE,5 1/2&quot;,5 1/2&quot;,4,9.52627&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,-25'3.18078&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-41'2&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

AppendRoofEdge(roofHandle,-77'10&quot;,21'4.81922&quot;,#45°0'0&quot;,2'0&quot;,10'0&quot;);

shedID := CreateShedDormer(roofHandle);

SetShedAttributes(roofHandle,shedID,TRUE,6'0&quot;,10'0&quot;,2'0&quot;,#8°0'0&quot;);

SetDormerAttributes(roofHandle, shedID, 3,18'4&quot;,TRUE,3'0&quot;,63,FALSE,3'0&quot;);

SetDormerThick(roofHandle, 2&quot;,1.83333&quot;);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


# SetDormerThick

## Description
Procedure SetDormerThick sets dormer roof and wall thicknesses for the referenced roof. 

```pascal
PROCEDURE SetDormerThick(
				roofObject        : HANDLE;
				wallThickDistance : REAL (Coordinate);
				roofThickDistance : REAL (Coordinate));
```

```python

def vs.SetDormerThick(roofObject, wallThickDistance, roofThickDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|wallThickDistance|REAL (Coordinate)|Wall thickness of dormer.|
|roofThickDistance|REAL (Coordinate)|Roof thickness of dormer.|

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


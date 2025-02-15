# CreateBatDormer

## Description
Function CreateBatDormer creates a bat dormer in the referenced roof object.

```pascal
FUNCTION CreateBatDormer(roofObject : HANDLE) : INTEGER;
```

```python

def vs.CreateBatDormer(roofObject):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|

## Remarks
This only creates the object, SetDormerAttributes() &amp; SetBatAttributes() must still be called to define the attributes of the dormer.<BR>
<BR>


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


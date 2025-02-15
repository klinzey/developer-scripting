# CreateSkylight

## Description
Function CreateSkylight creates a new skylight in the referenced roof object.

```pascal
FUNCTION CreateSkylight(roofObject : HANDLE) : INTEGER;
```

```python

def vs.CreateSkylight(roofObject):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|

## Examples
```pascal
skylightID:=CreateSkylight(roofHandle);

SetSkylight(roofHandle,skylightID,6,13'8&quot;,2'1&quot;,Name2Index('dh2436'));


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


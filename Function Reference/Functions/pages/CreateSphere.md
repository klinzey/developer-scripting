# CreateSphere

## Description
Function CreateSphere creates a new sphere object in a Vectorworks document.

```pascal
FUNCTION CreateSphere(
				center         : REAL;
				radiusDistance : REAL (Coordinate)) : HANDLE;
```

```python

def vs.CreateSphere(center, radiusDistance):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|center|REAL|Center point of sphere.|
|radiusDistance|REAL (Coordinate)|Radius of sphere.|

## Returns
The function returns a handle to the new sphere object.

## Remarks
[sd 8/18/98]

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Solids


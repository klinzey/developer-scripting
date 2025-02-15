# CreateCone

## Description
Creates a 3D cone object in a Vectorworks document.

```pascal
FUNCTION CreateCone(
				center         : REAL;
				tip            : REAL;
				radiusDistance : REAL (Coordinate)) : HANDLE;
```

```python

def vs.CreateCone(center, tip, radiusDistance):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|center|REAL|Center point of cone.|
|tip|REAL|Tip point of cone.|
|radiusDistance|REAL (Coordinate)|Radius of cone base.|

## Returns
The function returns a handle to the new cone object.

## Remarks
[sd 8/18/98]

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Solids


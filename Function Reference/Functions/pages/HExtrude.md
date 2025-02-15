# HExtrude

## Description
Creates an extrude object from the specified object.

```pascal
FUNCTION HExtrude(
				objectH : HANDLE;
				bottom  : REAL;
				top     : REAL) : HANDLE;
```

```python

def vs.HExtrude(objectH, bottom, top):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectH|HANDLE|The profile to be extruded.|
|bottom|REAL|The z height of the bottom of the extrude.|
|top|REAL|The z height of the top of the extrude.|

## Returns
A handle to the newly created extrude object.

## Version
Availability: from VectorWorks10.0
## Category
* Objects - 3D


# CreateTaperedExtrude

## Description
Creates a new tapered extrude object in the document.

```pascal
FUNCTION CreateTaperedExtrude(
				profileH : HANDLE;
				angle    : REAL;
				height   : REAL) : HANDLE;
```

```python

def vs.CreateTaperedExtrude(profileH, angle, height):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|profileH|HANDLE|Handle to object defining profile geometry.|
|angle|REAL|Taper angle of extrude (in degrees).|
|height|REAL|Height of extrude.|

## Returns
Returns a HANDLE to the new tapered extrude if successful, otherwise returns NIL.

## Version
Availability: from VectorWorks9.0
## Category
* Objects - 3D


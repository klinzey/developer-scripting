# CreateTaperedExtrd2

## Description
Creates a new tapered extrude object in the document. This function returns a &amp;quot;general solid&amp;quot; object while the other function, CreateTaperedExtrude, produces a bunch of NURBS surfaces.

```pascal
FUNCTION CreateTaperedExtrd2(
				profileH : HANDLE;
				angle    : REAL;
				height   : REAL) : HANDLE;
```

```python

def vs.CreateTaperedExtrd2(profileH, angle, height):
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
Availability: from Vectorworks 2016
## Category
* Objects - 3D


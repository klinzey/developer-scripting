# ClipSurfaceN

## Description
Creates a new surface object by subtracting the intersection of surfaces s1 and s2 from s1.

```pascal
FUNCTION ClipSurfaceN(
				s1 : HANDLE;
				s2 : HANDLE) : HANDLE;
```

```python

def vs.ClipSurfaceN(s1, s2):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|s1|HANDLE|Surface to be subtracted from|
|s2|HANDLE|Surface to subtract from s1|

## Version
Availability: from Vectorworks 2016
## Category
* Objects - 2D


# OLDSetHangPathHandle

## Description
Adds the path to the hang points of the specified load for the parametric object

```pascal
FUNCTION OLDSetHangPathHandle(
				handle           : HANDLE;
				loadIndex        : INTEGER;
				path             : HANDLE;
				height           : REAL;
				deletePathHandle : BOOLEAN) : REAL;
```

```python

def vs.OLDSetHangPathHandle(handle, loadIndex, path, height, deletePathHandle):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|handle|HANDLE||
|loadIndex|INTEGER||
|path|HANDLE||
|height|REAL||
|deletePathHandle|BOOLEAN||

## Version
Availability: from Vectorworks 2018
## Category
* Truss Analysis


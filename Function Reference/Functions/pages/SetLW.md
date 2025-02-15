# SetLW

## Description
Procedure SetLW sets the line weight of the referenced object.

```pascal
PROCEDURE SetLW(
				h  : HANDLE;
				lw : INTEGER);
```

```python

def vs.SetLW(h, lw):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object|
|lw|INTEGER|Line weight to be applied to object (in mils).|

## Examples
```pascal
SetLW(ObjHd,12);


```

## Version
Availability: from MiniCAD
## Category
* Object Attributes


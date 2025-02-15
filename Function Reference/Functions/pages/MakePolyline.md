# MakePolyline

## Description
Creates a polyline using inSourceObject. inSourceObject is unchanged.

```pascal
FUNCTION MakePolyline(inSourceObject : HANDLE) : HANDLE;
```

```python

def vs.MakePolyline(inSourceObject):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inSourceObject|HANDLE|The 2D object from which to make a polyline.|

## Returns
A polyline representation of inSourceObject.

## Remarks
Creates a polyline from inSourceObject. inSourceObject is unchanged.

## Examples
```pascal
PROCEDURE Example;

VAR

	h,h2:HANDLE;

BEGIN

h:=FSActLayer;

h2 := MakePolyline(h);

DelObject(h);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks10.1
## Category
* Objects - 2D


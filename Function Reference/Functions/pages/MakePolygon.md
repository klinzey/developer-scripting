# MakePolygon

## Description
MakePolygon creates a 2D Polygon using inSourceObject. Does not delete inSourceObject.

```pascal
FUNCTION MakePolygon(inSourceObject : HANDLE) : HANDLE;
```

```python

def vs.MakePolygon(inSourceObject):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inSourceObject|HANDLE|inSource object should be a 2D object that can be polygonalized.|

## Returns
A polygonalized copy of inSourceObject

## Examples
```pascal
PROCEDURE Example;

VAR

	h :HANDLE;

BEGIN

	CallTool(-204);

	h := FSActLayer;

	h := MakePolygon(h);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks10.1
## Category
* Objects - 2D


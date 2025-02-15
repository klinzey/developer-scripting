# ConvertToNURBS

## Description
This function converts the input object into a new NURBS object or a group of NURBS objects in the document.

```pascal
FUNCTION ConvertToNURBS(
				h        : HANDLE;
				keepOrig : BOOLEAN) : HANDLE;
```

```python

def vs.ConvertToNURBS(h, keepOrig):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle of original object.|
|keepOrig|BOOLEAN|Leave the original object in the drawing.|

## Examples
```pascal
PROCEDURE Example;

VAR

	h :handle;

BEGIN

	CallTool(-204);

	h := FSActLayer;

	h := ConvertToNURBS(h, false);

	h := CreateOffsetNurbsObjectHandle(h, 1);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks10.0
## Category
* Objects - NURBS


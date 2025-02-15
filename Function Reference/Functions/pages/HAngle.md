# HAngle

## Description
Function HAngle returns the angle of the referenced line or arc object.&lt;BR&gt;


```pascal
FUNCTION HAngle(h : HANDLE) : REAL;
```

```python

def vs.HAngle(h):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
PROCEDURE Example;

BEGIN

	CallTool(-202);

	Message(HAngle(FSActLayer));

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Object Info


# HMoveForward

## Description
Move the referenced object forward in the object stacking order. If toFront is TRUE, the object will be moved to the front of the stacking order.

```pascal
PROCEDURE HMoveForward(
				h       : HANDLE;
				toFront : BOOLEAN);
```

```python

def vs.HMoveForward(h, toFront):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|toFront|BOOLEAN|Move object to front of stacking order.|

## Examples
```pascal
PROCEDURE Example;

BEGIN

	HMoveForward(FSActLayer, FALSE);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks8.5
## Category
* Object Editing


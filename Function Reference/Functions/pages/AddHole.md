# AddHole

## Description
AddHole uses a holeTemplate to create a hole inside objectToGetHole.  Upon success, objectToGetHole is converted to polyline.   holeTemplate is unchanged.

```pascal
FUNCTION AddHole(
				VAR objectToGetHole : HANDLE;
				holeTemplate        : HANDLE) : BOOLEAN;
```

```python

def vs.AddHole(objectToGetHole, holeTemplate):
    return (BOOLEAN, objectToGetHole)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectToGetHole|HANDLE|A 2D object to be cut by holeTemplate.|
|holeTemplate|HANDLE|A 2D object to cut a hole out of objectToGetHole.|

## Examples
```pascal
PROCEDURE AddHoleExample;

VAR

	h1, h2 :HANDLE;

BEGIN

	CallTool(-204);

	h1 := FSActLayer;

	CallTool(-204);

	h2 := FSActLayer;

	IF AddHole(h1, h2) THEN SetFPat(h1, 3);

END;

RUN(AddHoleExample);


```

## Version
Availability: from VectorWorks10.1
## Category
* Objects - 2D


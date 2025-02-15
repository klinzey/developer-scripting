# SetName

## Description
Procedure SetName assigns a name to the referenced object.

```pascal
PROCEDURE SetName(
				h    : HANDLE;
				name : STRING);
```

```python

def vs.SetName(h, name):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|name|STRING|Name to be assigned to object.|

## Examples
```pascal
PROCEDURE Example;

VAR

	h1    :HANDLE;

	SName :STRING;

BEGIN

	SName := 'Fred';

	h1 := CreateSphere(0, 0, 0, 1000);

	SetName(h1, SName);

END;

RUN(Example);
```

## See Also
VS Functions:
[GetName](GetName.md)

## Version
Availability: from MiniCAD
## Category
* Object Names


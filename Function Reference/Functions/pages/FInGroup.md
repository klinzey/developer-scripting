# FInGroup

## Description
Function FInGroup returns a handle to the first component object of the referenced group.&lt;BR&gt;


```pascal
FUNCTION FInGroup(ObjectHd : HANDLE) : HANDLE;
```

```python

def vs.FInGroup(ObjectHd):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|ObjectHd|HANDLE|Handle to group object.|

## Examples
```pascal
PROCEDURE Example;

VAR

	h :HANDLE;

BEGIN

	h := FInGroup(FSActLayer);

	WHILE h &lt;&gt; NIL DO BEGIN

		SetClass(h, 'None');

		h := NextObj(h);

	END;

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Document List Handling


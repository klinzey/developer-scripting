# GetLW

## Description
Function GetLW returns the line weight of the referenced object. The value returned represents the width in mils.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetLW(h : HANDLE) : INTEGER;
```

```python

def vs.GetLW(h):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
PROCEDURE GetLWExample;

VAR

	x, y :REAL;

	h :HANDLE;

BEGIN

	GetPt(x, y);

	h := PickObject(x, y);

	IF h &lt;&gt; NIL THEN Message(GetLW(h));

END;

RUN(GetLWExample);


```

## Version
Availability: from MiniCAD
## Category
* Object Attributes


# Ord

## Description
Function Ord returns the corresponding ASCII number of the specified character value. Parameter Ord specifies the character.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Ord(v : CHAR) : INTEGER;
```

```python

def vs.Ord(v):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v|CHAR|ASCII character.|

## Examples
```pascal
PROCEDURE Main;

VAR

	str :STRING;

	cnt :INTEGER;

BEGIN

	str := GetText(FSActLayer);

	FOR cnt := 1 TO Len(str) DO

		AlrtDialog(Concat(Ord(Copy(str, cnt, 1))));

END;

RUN(Main);
```

## See Also
VS Functions:
[Chr](Chr.md)

## Version
Availability: from MiniCAD
## Category
* Strings


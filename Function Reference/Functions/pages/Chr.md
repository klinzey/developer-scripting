# Chr

## Description
Function Chr returns the ASCII character corresponding to the specified numeric code. The ASCII code value must be between 1 and 255.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Chr(v : INTEGER) : CHAR;
```

```python

def vs.Chr(v):
    return CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v|INTEGER|ASCII numeric identifier code.|

## Examples
```pascal
PROCEDURE Example;

VAR

	cnt :INTEGER;

	str :STRING;

BEGIN

	FOR cnt := 128 TO 255 DO BEGIN

		str := Concat(str, Chr(cnt));

		IF cnt MOD 32 = 0 THEN str := Concat(str, Chr(13));

	END;

	AlrtDialog(str);

END;

RUN(Example);


```

## See Also
VS Functions:
[Ord](Ord.md)

## Version
Availability: from MiniCAD
## Category
* Strings


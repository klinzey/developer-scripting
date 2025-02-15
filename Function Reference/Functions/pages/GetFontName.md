# GetFontName

## Description
Function GetFontName converts a system font ID to a font name.&lt;BR&gt;
&lt;BR&gt;
An integer ID with a value representing a font in the current operating system.

```pascal
FUNCTION GetFontName(fontID : INTEGER) : STRING;
```

```python

def vs.GetFontName(fontID):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fontID|INTEGER|Font ID value.|

## Remarks
returns &quot;&quot; if the FontID is not legal.

## Examples
```pascal
PROCEDURE Example;

VAR

	str :STRING;

	cnt :INTEGER;

BEGIN

	FOR cnt := 0 to 10 DO str := Concat(str, Chr(13), GetFontName(cnt));

	AlrtDialog(str);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text


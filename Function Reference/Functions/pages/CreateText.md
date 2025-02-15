# CreateText

## Description
Procedure CreateText creates a new text object in a Vectorworks document. The text object is created using the current pen position and default attributes.

```pascal
PROCEDURE CreateText(theText : DYNARRAY[] of CHAR);
```

```python

def vs.CreateText(theText):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theText|DYNARRAY[] of CHAR|Text string.|

## Examples
```pascal
PROCEDURE Example;

VAR

	Txt   :ARRAY [1..100] of STRING;

	Outpt :DYNARRAY[] of CHAR;

	i     :INTEGER;

BEGIN

	FOR i := 1 TO 5 DO txt[i] := 'asdf';

	i := 2;

	Outpt := Txt[1];

	WHILE Txt[i] &lt;&gt; '' DO BEGIN

		OutPt := Concat(Outpt, Chr(13), Txt[i]);

		i := i + 1;

	END;

	Layer('Text');

	CreateText(Outpt);

	Layer('Layer-1');

END;

RUN(Example);
```

## See Also
VS Functions:
[BeginText](BeginText.md)| [EndText](EndText.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text


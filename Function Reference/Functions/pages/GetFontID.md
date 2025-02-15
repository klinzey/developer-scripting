# GetFontID

## Description
Function GetFontID converts the string name of an available font to a font ID which can be passed to other VectorScript routines.

```pascal
FUNCTION GetFontID(fontName : STRING) : INTEGER;
```

```python

def vs.GetFontID(fontName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fontName|STRING|Name of installed font.|

## Remarks
returns -1 if the requested font is not available

## Examples
```pascal
PROCEDURE Example;

VAR

	str :STRING;

BEGIN

	str := StrDialog('Enter the font name:', 'Arial');

	AlrtDialog(Concat('The font ID is: ', GetFontID(str)));

END;

RUN(Example);
```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text


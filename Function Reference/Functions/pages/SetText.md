# SetText

## Description
Procedure SetText sets the content of the referenced text object. The new text is assigned the font, size and style characteristics of the first character of the old text string.

```pascal
PROCEDURE SetText(
				objectHd : HANDLE;
				text     : DYNARRAY[] of CHAR);
```

```python

def vs.SetText(objectHd, text):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to text object.|
|text|DYNARRAY[] of CHAR|New text string value.|

## Examples
```pascal
SetText(hText,'A new text string value');
```

## Version
Availability: from MiniCAD
## Category
* Objects - Text


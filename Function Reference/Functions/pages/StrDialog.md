# StrDialog

## Description
Function StrDialog, displays a dialog box which requests the user to enter a string value.&lt;BR&gt;


```pascal
FUNCTION StrDialog(
				request : DYNARRAY[] of CHAR;
				default : DYNARRAY[] of CHAR) : STRING;
```

```python

def vs.StrDialog(request, default):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|default|DYNARRAY[] of CHAR|Default value for input field.|

## Examples
```pascal
PROCEDURE Example;

VAR

   request, default, result :STRING;

BEGIN

   request := 'Enter some text...';

   default := 'the default value';

   result := StrDialog(request, default);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


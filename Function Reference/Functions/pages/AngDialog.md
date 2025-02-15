# AngDialog

## Description
Function AngDialog displays a dialog box which requests the user to enter an angle value. The dialog automatically screens for valid numeric input, and will accept supported angle formats.

```pascal
FUNCTION AngDialog(
				request : DYNARRAY[] of CHAR;
				default : DYNARRAY[] of CHAR) : REAL;
```

```python

def vs.AngDialog(request, default):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|default|DYNARRAY[] of CHAR|Default value for input field.|

## Examples
```pascal
AngleValue := AngDialog('Enter an angle value:', '0d');
```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


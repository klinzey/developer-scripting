# YNDialog

## Description
Function YNDialog displays a dialog box which requests the user to select a Yes or No value. If the user selects the Yes button in the dialog box, the value returned by YNDialog is TRUE; if the user selects No, the function returns FALSE.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION YNDialog(s : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.YNDialog(s):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|s|DYNARRAY[] of CHAR|Dialog user prompt string.|

## Examples
```pascal
Answer := YNDialog('Do you wish to continue');


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


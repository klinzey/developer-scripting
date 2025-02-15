# PtDialog

## Description
Procedure PtDialog displays a dialog box which requests the user to enter a coordinate (point) value.&lt;BR&gt;


```pascal
PROCEDURE PtDialog(
				request  : DYNARRAY[] of CHAR;
				defaultX : DYNARRAY[] of CHAR;
				defaultY : DYNARRAY[] of CHAR;
				VAR x    : REAL;
				VAR y    : REAL);
```

```python

def vs.PtDialog(request, defaultX, defaultY):
    return (x, y)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|defaultX|DYNARRAY[] of CHAR|Default value for input field.|
|defaultY|DYNARRAY[] of CHAR|Default value for input field.|
|x|REAL|Returns user input X value.|
|y|REAL|Returns user input Y value.|

## Examples
```pascal
PtDialog('Enter a coordinate.','0','0',cX,cY);


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


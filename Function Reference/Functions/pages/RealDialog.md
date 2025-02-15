# RealDialog

## Description
Function RealDialog displays a dialog box which requests the user to enter a REAL value. RealDialog automatically screens for valid numeric input.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION RealDialog(
				request : DYNARRAY[] of CHAR;
				default : DYNARRAY[] of CHAR) : REAL;
```

```python

def vs.RealDialog(request, default):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|default|DYNARRAY[] of CHAR|Default value for input field.|

## Examples
```pascal
RealValue:=RealDialog('Enter a real value:','0.00');


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


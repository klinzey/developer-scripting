# DistDialog

## Description
Function DistDialog displays a dialog box which requests the user to enter a distance value.&lt;BR&gt;
&lt;BR&gt;
DistDialog automatically screens for valid numeric input.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION DistDialog(
				request : DYNARRAY[] of CHAR;
				default : DYNARRAY[] of CHAR) : REAL;
```

```python

def vs.DistDialog(request, default):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|default|DYNARRAY[] of CHAR|Default value for input field.|

## Examples
```pascal
DistValue := DistDialog('Enter a distance value:','0');


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


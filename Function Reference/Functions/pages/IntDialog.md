# IntDialog

## Description
Function IntDialog displays a dialog box which requests the user to enter an integer value. &lt;BR&gt;
&lt;BR&gt;
IntDialog automatically screens for valid numeric input.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION IntDialog(
				request : DYNARRAY[] of CHAR;
				default : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.IntDialog(request, default):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|request|DYNARRAY[] of CHAR|Dialog user prompt string.|
|default|DYNARRAY[] of CHAR|Default value for input field.|

## Examples
```pascal
distValue := IntDialog('Enter an integer value:','0');


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined


# SetLBColumnWidth

## Description
Sets the width of the specified range of columns of the specified list browser control.

```pascal
FUNCTION SetLBColumnWidth(
				dialogID    : LONGINT;
				componentID : LONGINT;
				fromColumn  : INTEGER;
				toColumn    : INTEGER;
				width       : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBColumnWidth(dialogID, componentID, fromColumn, toColumn, width):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|fromColumn|INTEGER|first column to be changed|
|toColumn|INTEGER|last column to be changed|
|width|INTEGER|the width of the column in pixels|

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


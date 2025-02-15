# GetIconPushButtonState

## Description
Retrieves the state of the specified Layout Manager icon push button (pressed or not pressed).

```pascal
FUNCTION GetIconPushButtonState(
				nDialogID    : LONGINT;
				nComponentID : LONGINT;
				VAR bPressed : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetIconPushButtonState(nDialogID, nComponentID):
    return (BOOLEAN, bPressed)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|nDialogID|LONGINT||
|nComponentID|LONGINT||
|bPressed|BOOLEAN||

## Version
Availability: from VectorWorks 2008
## Category
* Dialogs - Modern


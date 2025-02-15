# SetHelpText

## Description
Sets the help text for the given component.

```pascal
PROCEDURE SetHelpText(
				dialogID    : LONGINT;
				componentID : LONGINT;
				helpText    : DYNARRAY[] of CHAR);
```

```python

def vs.SetHelpText(dialogID, componentID, helpText):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the dialog identifier given by CreateLayout or CreateResizableLayout|
|componentID|LONGINT|The identifier of the component for which to set the help text.|
|helpText|DYNARRAY[] of CHAR|The help text to set for the given component.|

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Modern


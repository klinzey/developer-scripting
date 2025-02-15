# RunLayoutDialog

## Description
Displays the specified dialog and initiates the dialog event loop. The dialog event loop is specified in a procedure subroutine that is passed as a parameter to the function.

```pascal
FUNCTION RunLayoutDialog(
				dialogID : LONGINT;
				callback : PROCEDURE) : LONGINT;
```

```python

def vs.RunLayoutDialog(dialogID, callback):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog to be displayed.|
|callback|PROCEDURE|The event loop subroutine for the dialog.|

## Returns
Returns a LONGINT value indicating the button pressed to exit the dialog.

## Remarks
[DWD 1/20/00]

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


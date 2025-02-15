# CreatePullDownMenu

## Description
Creates a new pulldown menu control in a dialog layout.

```pascal
PROCEDURE CreatePullDownMenu(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				widthInStdChar : LONGINT);
```

```python

def vs.CreatePullDownMenu(dialogID, itemID, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Remarks
[DWD 1/20/00]

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


# CreateListBox

## Description
Creates a new list box control in a dialog layout.

```pascal
PROCEDURE CreateListBox(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				widthInStdChar : LONGINT;
				heightInLines  : LONGINT);
```

```python

def vs.CreateListBox(dialogID, itemID, widthInStdChar, heightInLines):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|heightInLines|LONGINT|The height of the control in characters.|

## Remarks
[DWD 1/20/00]

## Examples
```pascal
{ draws a list box 25 characters wide and 7 rows high }

CreateListBox(2,10,25,7);


```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


# CreateListBoxN

## Description
Creates a new list box control in a dialog layout. With isMultipleSelect true, the list supports multiple selection.

```pascal
PROCEDURE CreateListBoxN(
				dialogID         : LONGINT;
				itemID           : LONGINT;
				widthInStdChar   : LONGINT;
				heightInLines    : LONGINT;
				isMultipleSelect : BOOLEAN);
```

```python

def vs.CreateListBoxN(dialogID, itemID, widthInStdChar, heightInLines, isMultipleSelect):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|heightInLines|LONGINT|The height of the control in characters.|
|isMultipleSelect|BOOLEAN|Does the list support multiple selection|

## Examples
```pascal
{ draws a muliple selection list box 25 characters wide and 7 rows high }

CreateListBoxN(2,10,25,7, true);


```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks10.5
## Category
* Dialogs - Modern


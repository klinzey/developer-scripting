# CreateLB

## Description
Creates a layout manager list browser control.

```pascal
PROCEDURE CreateLB(
				dialogID       : LONGINT;
				componentID    : LONGINT;
				widthInStdChar : INTEGER;
				heightInLines  : INTEGER);
```

```python

def vs.CreateLB(dialogID, componentID, widthInStdChar, heightInLines):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|heightInLines|INTEGER|the height of the control in characters|

## Remarks
Parser.Execute.cpp

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


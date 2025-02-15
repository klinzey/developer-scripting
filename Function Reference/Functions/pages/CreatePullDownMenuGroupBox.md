# CreatePullDownMenuGroupBox

## Description
Creates a Layout Manager pull down menu group box.

```pascal
PROCEDURE CreatePullDownMenuGroupBox(
				liDialogID     : LONGINT;
				liComponentID  : LONGINT;
				widthInStdChar : INTEGER;
				strLabel       : STRING;
				bHasFrame      : BOOLEAN);
```

```python

def vs.CreatePullDownMenuGroupBox(liDialogID, liComponentID, widthInStdChar, strLabel, bHasFrame):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|liDialogID|LONGINT||
|liComponentID|LONGINT||
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|strLabel|STRING||
|bHasFrame|BOOLEAN||

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks12.5
## Category
* Dialogs - Modern


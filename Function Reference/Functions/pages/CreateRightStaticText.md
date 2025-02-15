# CreateRightStaticText

## Description
Similar to CreateStaticText, but creates static text that is right-justified in its control field on the dialog.

```pascal
PROCEDURE CreateRightStaticText(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				text           : STRING;
				widthInStdChar : INTEGER);
```

```python

def vs.CreateRightStaticText(dialogID, itemID, text, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|text|STRING||
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks12.0.1
## Category
* Dialogs - Modern


# CreateCenteredStaticText

## Description
Similar to CreateStaticText, but creates static text that is centered in its control field on the dialog.

```pascal
PROCEDURE CreateCenteredStaticText(
				dialogID       : LONGINT;
				controlID      : LONGINT;
				text           : STRING;
				widthInStdChar : INTEGER);
```

```python

def vs.CreateCenteredStaticText(dialogID, controlID, text, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|controlID|LONGINT||
|text|STRING||
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks12.0.1
## Category
* Dialogs - Modern


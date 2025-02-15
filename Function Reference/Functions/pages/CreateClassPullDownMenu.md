# CreateClassPullDownMenu

## Description
Creates a Layout Manager class pull down menu control.

```pascal
PROCEDURE CreateClassPullDownMenu(
				nDialogID      : LONGINT;
				nComponentID   : LONGINT;
				widthInStdChar : INTEGER);
```

```python

def vs.CreateClassPullDownMenu(nDialogID, nComponentID, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|nDialogID|LONGINT||
|nComponentID|LONGINT||
|widthInStdChar|INTEGER|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Examples
```pascal
PROCEDURE Example;

VAR

   dialog1 :INTEGER;

   result  :INTEGER;

PROCEDURE Dialog_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

END;

BEGIN

   dialog1 := CreateLayout('Example Dialog', FALSE, 'OK', 'Cancel');

   CreateClassPullDownMenu(dialog1, 4, 24);

   SetFirstLayoutItem(dialog1, 4);

   result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);
```

## See Also
VS Functions:
[CreateImageControl](CreateImageControl.md)| [GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks 2008
## Category
* Dialogs - Modern


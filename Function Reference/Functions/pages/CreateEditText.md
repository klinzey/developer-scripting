# CreateEditText

## Description
Creates an editable text field control in a dialog layout.

```pascal
PROCEDURE CreateEditText(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				defaultText    : STRING;
				widthInStdChar : LONGINT);
```

```python

def vs.CreateEditText(dialogID, itemID, defaultText, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|defaultText|STRING|The default display text for the control.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Remarks
[DWD 1/20/00]

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

	CreateEditText(dialog1, 4, 'default text', 16);

	SetFirstLayoutItem(dialog1, 4);

	result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);




```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


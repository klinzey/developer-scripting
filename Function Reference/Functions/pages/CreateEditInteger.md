# CreateEditInteger

## Description
Creates an editable text field control for INTEGER and LONGINT values.&lt;BR&gt;
&lt;BR&gt;
CreateEditInteger is intended specifically for entry of numeric values; the control returns values in a numeric format, and supports calculations within the control field.

```pascal
PROCEDURE CreateEditInteger(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				defaultValue   : LONGINT;
				widthInStdChar : LONGINT);
```

```python

def vs.CreateEditInteger(dialogID, itemID, defaultValue, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|defaultValue|LONGINT|Default value for the field.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|

## Remarks
Edits long ints, does math,  get and set values with get and set integer calls[DWD 11/20/00]

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

	CreateEditInteger(dialog1, 4, 123, 16);

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


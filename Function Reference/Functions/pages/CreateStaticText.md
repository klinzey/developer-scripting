# CreateStaticText

## Description
Creates a new static text field control in a dialog layout.&lt;BR&gt;
&lt;BR&gt;
To allow the control to size automatically to the text width, pass -1 as the width parameter of the control.

```pascal
PROCEDURE CreateStaticText(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				text           : STRING;
				widthInStdChar : LONGINT);
```

```python

def vs.CreateStaticText(dialogID, itemID, text, widthInStdChar):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|text|STRING|The display text for the control.|
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

   CreateStaticText(dialog1, 5, 'default text', 16);

   SetFirstLayoutItem(dialog1, 4);

   SetBelowItem(dialog1, 4, 5, 0, 0);

   result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[CreateStyledStatic](CreateStyledStatic.md)| [GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


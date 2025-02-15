# CreateEditTextBox

## Description
Creates a scrolling multiline editable text field in a dialog layout. 

```pascal
PROCEDURE CreateEditTextBox(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				defaultText    : STRING;
				widthInStdChar : LONGINT;
				heightInLines  : LONGINT);
```

```python

def vs.CreateEditTextBox(dialogID, itemID, defaultText, widthInStdChar, heightInLines):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The id of the dialog|
|itemID|LONGINT|The id of the text box control. |
|defaultText|STRING|The initial text.|
|widthInStdChar|LONGINT|The width of the displayed text in standard character count. See GetDlgCtrlWidthStdCh.|
|heightInLines|LONGINT|Height of the control in lines. |

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

	CreateEditTextBox(dialog1, 4, 'default text', 24, 16);

	SetFirstLayoutItem(dialog1, 4);

	result := RunLayoutDialog(dialog1, Dialog_Handler);

END;

RUN(Example);


```

## See Also
VS Functions:
[GetDlgCtrlWidthStdCh](GetDlgCtrlWidthStdCh.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


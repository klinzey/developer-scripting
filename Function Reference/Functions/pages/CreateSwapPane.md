# CreateSwapPane

## Description
Creates a swap pane within the specified swap control.   Within a swap control, only one swap pane is visible at a time.

```pascal
PROCEDURE CreateSwapPane(
				dialogID      : LONGINT;
				swapControlID : LONGINT;
				newGroupID    : LONGINT);
```

```python

def vs.CreateSwapPane(dialogID, swapControlID, newGroupID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the ID of the dialog|
|swapControlID|LONGINT|the ID of the swap control|
|newGroupID|LONGINT|the ID of the group to be inserted into swap control as a swap pane.|

## Remarks
The function is analogous to CreateTabPane.

## Examples
```pascal
PROCEDURE dialog1_Main;

CONST

	kOK            = 1;

	kCancel        = 2;

	kTabControl    = 4;

	kTabPane_1     = 5;

	kTabPane_2     = 6;

	kSwapControl_1 = 7;

	kSwapControl_2 = 8;

	kSwapPane_11   = 9;

	kSwapPane_21   = 10;

	kSwapPane_12   = 11;

	kSwapPane_22   = 12;

	kButton_11     = 13;

	kButton_21     = 14;

	kButton_12     = 15;

	kButton_22     = 16;

VAR

	dialog1          :INTEGER;



PROCEDURE dialog1_Setup;

BEGIN

	dialog1 := CreateLayout('Tabs and Swaps', False, 'OK', 'Cancel');

	CreateTabControl         (dialog1, kTabControl);

	CreateGroupBox           (dialog1, kTabPane_1,      'Tab Pane 1', True);

	CreateGroupBox           (dialog1, kTabPane_2,      'Tab Pane 2', True);

	CreateSwapControl        (dialog1, kSwapControl_1);

	CreateSwapControl        (dialog1, kSwapControl_2);

	CreateGroupBox           (dialog1, kSwapPane_11,    '', True);

	CreateGroupBox           (dialog1, kSwapPane_21,    '', True);

	CreateGroupBox           (dialog1, kSwapPane_12,    '', True);

	CreateGroupBox           (dialog1, kSwapPane_22,    '', True);

	CreatePushButton         (dialog1, kButton_11,      'Button 1');

	CreatePushButton         (dialog1, kButton_21,      'Button 3');

	CreatePushButton         (dialog1, kButton_12,      'Button 2');

	CreatePushButton         (dialog1, kButton_22,      'Button 4');



	SetFirstLayoutItem(dialog1, kTabControl);

	CreateTabPane     (dialog1, kTabControl,     kTabPane_1);

	SetFirstGroupItem (dialog1, kTabPane_1,      kSwapControl_1);

	CreateSwapPane    (dialog1, kSwapControl_1,  kSwapPane_11);

	SetFirstGroupItem (dialog1, kSwapPane_11,    kButton_11);

	CreateSwapPane    (dialog1, kSwapControl_1,  kSwapPane_12);

	SetFirstGroupItem (dialog1, kSwapPane_12,    kButton_12);

	CreateTabPane     (dialog1, kTabControl,     kTabPane_2);

	SetFirstGroupItem (dialog1, kTabPane_2,      kSwapControl_2);

	CreateSwapPane    (dialog1, kSwapControl_2,  kSwapPane_21);

	SetFirstGroupItem (dialog1, kSwapPane_21,    kButton_21);

	CreateSwapPane    (dialog1, kSwapControl_2,  kSwapPane_22);

	SetFirstGroupItem (dialog1, kSwapPane_22,    kButton_22);

END;



PROCEDURE dialog1_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

END;



BEGIN

	dialog1_Setup;

	IF RunLayoutDialog(dialog1, dialog1_Handler) = 1 then BEGIN

	END;

END;

RUN(dialog1_Main);


```

## See Also
VS Functions:
[CreateSwapControl](CreateSwapControl.md)| [DisplaySwapPane](DisplaySwapPane.md)

## Version
Availability: from VectorWorks11.5
## Category
* Dialogs - Modern


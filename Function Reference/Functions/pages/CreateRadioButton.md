# CreateRadioButton

## Description
Creates a new radio button control in a dialog layout.&lt;BR&gt;
&lt;BR&gt;
Radio button groups can be created by defining two or more radio buttons with consecutive index values. When defined as a button group, VectorScript will handle selection-deselection of controls within the group.

```pascal
PROCEDURE CreateRadioButton(
				dialogID : LONGINT;
				itemID   : LONGINT;
				text     : STRING);
```

```python

def vs.CreateRadioButton(dialogID, itemID, text):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|text|STRING|The display text for the control.|

## Remarks
[DWD 1/20/00]

## Examples
```pascal
{ creates a radio button with the specified label }

	CreateRadioButton(lEditID,8,'Visible');



	CreateRadioButton(lEditID,9,'Grayed');

	CreateRadioButton(lEditID,10,'Hidden');

	CreateStaticText( lEditID,11,'',6); 


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


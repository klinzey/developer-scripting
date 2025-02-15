# CreateLayout

## Description
Creates a new custom dialog layout. After the layout is created, control items for the dialog can be added to the layout.

```pascal
FUNCTION CreateLayout(
				dialogTitle       : STRING;
				hasHelp           : BOOLEAN;
				defaultButtonName : STRING;
				cancelButtonName  : STRING) : LONGINT;
```

```python

def vs.CreateLayout(dialogTitle, hasHelp, defaultButtonName, cancelButtonName):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogTitle|STRING|Title of the dialog.|
|hasHelp|BOOLEAN|Enables help text for the dialog.|
|defaultButtonName|STRING|Text displayed in the default button of the dialog.|
|cancelButtonName|STRING|Text displayed in the cancel button of the dialog.|

## Returns
Returns an index number identifying the new dialog layout.

## Remarks
Creates a dialog with a default button, cancel button, and a help box. If you do not want a button created then pass an empty string. You can place your own default button simply by creating a button with ID 1.

## Examples
```pascal
{ creates a new dialog layout }

	lEditID := CreateLayout('Edit Layer',TRUE,'OK','Cancel');



	CreateGroupBox(lEditID,4,'',FALSE);

	CreateStaticText(lEditID,5,'Layer Name:',-1);

	CreateEditText(lEditID,6,'Layer-1',36);



	CreateGroupBox(lEditID,7,'Visibility',TRUE);

	CreateRadioButton(lEditID,8,'Visible');

	CreateRadioButton(lEditID,9,'Grayed');

	CreateRadioButton(lEditID,10,'Hidden');

	CreateStaticText( lEditID,11,'',6); 



	CreateGroupBox(lEditID,12,'Options',TRUE);

	CreateCheckBox(lEditID,13,'Use layer colors');

	CreateCheckBox(lEditID,14,'Create link on model layer');


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


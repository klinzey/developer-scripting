# CreateStandardIconControl

## Description
Creates a standard icon control, which is used to display the application icon or an alert icon. Valid values for iconNumber are:&lt;BR&gt;
0 - Vectorworks application icon&lt;BR&gt;
1 - Informational icon&lt;BR&gt;
2 - Stop icon&lt;BR&gt;
3 - Exclamation mark (warning) icon&lt;BR&gt;
4 - Question icon

```pascal
PROCEDURE CreateStandardIconControl(
				dialogID      : LONGINT;
				iconControlID : LONGINT;
				iconNumber    : INTEGER);
```

```python

def vs.CreateStandardIconControl(dialogID, iconControlID, iconNumber):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|ID of the dialog|
|iconControlID|LONGINT|ID of the control within the dialog|
|iconNumber|INTEGER|Constant, listed above, indicating which icon to display.|

## Remarks
Should show image of each icon.

## Examples
```pascal
dlog := CreateLayout('Untitled Dialog', False, 'OK', 'Cancel');



	CreateStandardIconControl(dlog, 4, 0);

	SetFirstLayoutItem(dlog, 4);



	result := RunLayoutDialog(dlog, EventHandler);




```

## Version
Availability: from VectorWorks11.5
## Category
* Dialogs - Modern


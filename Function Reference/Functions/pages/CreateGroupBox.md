# CreateGroupBox

## Description
Creates a new group box control in a dialog layout.&lt;BR&gt;
&lt;BR&gt;
The width of a group box is determined by the width of the longest control enclosed by the group box. The height of the group box is determined by the combined height of the enclosed controls.&lt;BR&gt;
&lt;BR&gt;
While used primarily to contain and highlight related control items, group box controls can also be used to group controls for easier positioning. When used in this fashion, pass a blank string for the display text and set the frame display to FALSE.

```pascal
PROCEDURE CreateGroupBox(
				dialogID : LONGINT;
				itemID   : LONGINT;
				text     : STRING;
				hasFrame : BOOLEAN);
```

```python

def vs.CreateGroupBox(dialogID, itemID, text, hasFrame):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout containing the control.|
|itemID|LONGINT|The index that will identify the control item.|
|text|STRING|The display text for the control.|
|hasFrame|BOOLEAN|Displays a border for the group box.|

## Remarks
A group box with out frame is used for placing and moving groups of controls.[DWG 1/20/00]

## Examples
```pascal
{ creates a framed group box entitled &quot;Options&quot; }

	CreateGroupBox(lEditID,12,'Options',TRUE);



	CreateCheckBox(lEditID,13,'Use layer colors');

	CreateCheckBox(lEditID,14,'Create link on model layer');


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


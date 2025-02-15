# CreateTabControl

## Description
Creates a tab control within a dialog.  The tab control manages the display of multiple panes of information and provides tab buttons that allow the user to swtich between panes. &lt;BR&gt;
&lt;BR&gt;
To create a tab control in a dialog, first define a group for each tab pane.  Add other controls to the groups and arrange them.  Then call CreateTabControl with an id.  Finally, call CreateTabPane for each pane providing the id of the group that defines that pane.  &lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE CreateTabControl(
				dialogID : LONGINT;
				itemID   : LONGINT);
```

```python

def vs.CreateTabControl(dialogID, itemID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The id of the dialog that contains this Tab control.|
|itemID|LONGINT|The id of the Tab control.|

## Examples
```pascal
Procedure TabControls;



const

	kTabControlID = 10;

	kTabPaneID1 = 20;

	kTabPaneID2 = 30;

	kTabPaneID3	= 40;

	

var

	dlogID, result  : LONGINT;

	

Procedure DialogProc(VAR item: LONGINT; data: LONGINT);

begin

	case item of

		SetupDialogC:

			begin

				result := 0;

			end;



		end;

end;



begin

	dlogID := CreateLayout('Sample Tab Dialog', false, 'OK', 'Cancel');



	{ Tab Group 1 }

	CreateGroupBox(dlogID, kTabPaneID1, 'Tab 1', FALSE);

	

	CreatePushButton(dlogID, 21, 'Button 1');

	SetFirstGroupItem(dlogID, kTabPaneID1, 21);	

	CreatePushButton(dlogID, 22, 'Button 2');

	SetBelowItem(dlogID, 21, 22, 0, 0);

	CreatePushButton(dlogID, 23, 'Button 3');

	SetBelowItem(dlogID, 22, 23, 0, 0);

	

	

	{ Tab Group 2 }

	CreateGroupBox(dlogID, kTabPaneID2, 'Tab 2', FALSE);

	

	CreatePushButton(dlogID, 31, 'Button 4');

	SetFirstGroupItem(dlogID, kTabPaneID2, 31);

	CreatePushButton(dlogID, 32, 'Button 5');

	SetRightItem(dlogID, 31, 32, 0, 0);

	CreatePushButton(dlogID, 33, 'Button 6');

	SetRightItem(dlogID, 32, 33, 0, 0);

	

	

	{ Tab Group 3 }

	CreateGroupBox(dlogID, kTabPaneID3, 'Tab 3', FALSE);

	

	CreatePushButton(dlogID, 41, 'Button 7');

	SetFirstGroupItem(dlogID, kTabPaneID3, 41);

	CreatePushButton(dlogID, 42, 'Button 8');

	SetRightItem(dlogID, 41, 42, 0, 0);

	CreatePushButton(dlogID, 43, 'Button 9');

	SetBelowItem(dlogID, 42, 43, 0, 0);

	



	{ Create tab control 1 }

	CreateTabControl(dlogID, kTabControlID);

	SetFirstLayoutItem(dlogID, kTabControlID);

	

	{ Add the tab panes to tab control }

	CreateTabPane(dlogID, kTabControlID, kTabPaneID1);

	CreateTabPane(dlogID, kTabControlID, kTabPaneID2);

	CreateTabPane(dlogID, kTabControlID, kTabPaneID3);

	

	result := RunLayoutDialog(dlogID, DialogProc);

end;

Run(TabControls);
```

## See Also
VS Functions:
[CreateTabPane](CreateTabPane.md)| [CreateGroupBox](CreateGroupBox.md)| [RunLayoutDialog](RunLayoutDialog.md)

## Version
Availability: from VectorWorks10.5
## Category
* Dialogs - Modern


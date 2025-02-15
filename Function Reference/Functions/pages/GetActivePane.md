# GetActivePane

## Description
Returns the currently displayed tab or swap pane in the specified tab or swap control. &lt;BR&gt;
&lt;BR&gt;
This is called from the dialog's event handling routine.

```pascal
FUNCTION GetActivePane(
				dialogID     : LONGINT;
				tabControlID : LONGINT) : LONGINT;
```

```python

def vs.GetActivePane(dialogID, tabControlID):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the ID of the dialog|
|tabControlID|LONGINT|the ID of the swap control|

## Remarks
Note that pane indeces are 1-based in VectorScript, and 0-based in the SDK.  Panes are numbered sequentially in the order that they were inserted into the control.  This applies to both tab and swap controls.

## Examples
```pascal
Procedure DialogProc(VAR item: LONGINT; data: LONGINT);

BEGIN

	CASE item OF

		SetupDialogC:

		BEGIN

			result := 0;

		END;



		100:	DisplaySwapPane(dlogID, 10, 1);  { Display pane 1 }

		101:	DisplaySwapPane(dlogID, 10, 2);  { Display pane 2 }

		102:	DisplaySwapPane(dlogID, 10, 3);  { Display pane 3 }



	END;

END;


```

## See Also
VS Functions:
[CreateSwapControl](CreateSwapControl.md)| [CreateSwapPane](CreateSwapPane.md)

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


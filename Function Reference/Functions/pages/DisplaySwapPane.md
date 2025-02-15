# DisplaySwapPane

## Description
Causes the specified swap pane to be displayed within the specified swap control. &lt;BR&gt;
&lt;BR&gt;
This is called from the dialog's event handling routine.

```pascal
PROCEDURE DisplaySwapPane(
				dialogID      : LONGINT;
				swapControlID : LONGINT;
				groupNumber   : LONGINT);
```

```python

def vs.DisplaySwapPane(dialogID, swapControlID, groupNumber):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the ID of the dialog|
|swapControlID|LONGINT|the ID of the swap control|
|groupNumber|LONGINT|1-based index of the swap pane to be displayed|

## Remarks
Note that pane indeces are 1-based in VectorScript, and 0-based in the SDK.  Swap panes are numbered sequentially in the order that they were inserted into the control.

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
Availability: from VectorWorks11.5
## Category
* Dialogs - Modern


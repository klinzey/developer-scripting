# SetLayoutDialogPosition

## Description
This function moves the dialog window to the given location.  Call this function to override the default automatic positioning of the dialog window.  The dialog will be pinned so that it is at least partly onscreen.&lt;BR&gt;
&lt;BR&gt;
This function can be useful for displaying a dialog in a position in which it was placed during prior use.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION SetLayoutDialogPosition(
				dialogID : LONGINT;
				left     : INTEGER;
				top      : INTEGER) : BOOLEAN;
```

```python

def vs.SetLayoutDialogPosition(dialogID, left, top):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index of the dialog.|
|left|INTEGER|Location of left edge of dialog in pixels.|
|top|INTEGER|Location of top edge of dialog in pixels.|

## Returns
true - success - the dialog window was moved.<BR>
false - failure - the dialog window was not moved, likely because it does not currently exist, or the dialogID is invalid.  The dialog window will exist anytime between the Setup message and OK/Cancel message.

## See Also
VS Functions:
[GetLayoutDialogPosition](GetLayoutDialogPosition.md)

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern


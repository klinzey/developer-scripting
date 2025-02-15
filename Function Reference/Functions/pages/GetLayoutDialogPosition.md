# GetLayoutDialogPosition

## Description
This function will retrieve the screen location of the dialog window, in pixels.&lt;BR&gt;
&lt;BR&gt;
This function can be useful for displaying a dialog in a position in which it was placed during prior use.

```pascal
FUNCTION GetLayoutDialogPosition(
				dialogID   : LONGINT;
				VAR left   : INTEGER;
				VAR top    : INTEGER;
				VAR right  : INTEGER;
				VAR bottom : INTEGER) : BOOLEAN;
```

```python

def vs.GetLayoutDialogPosition(dialogID):
    return (BOOLEAN, left, top, right, bottom)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index of the dialog.|
|left|INTEGER|Location of left edge of dialog, in pixels.|
|top|INTEGER|Location of top of dialog, in pixels.|
|right|INTEGER|Location of right edge of dialog, in pixels.|
|bottom|INTEGER|Location of bottom edge of dialog, in pixels.|

## Returns
true - success - the location of the dialog window was retrieved.<BR>
false - failure - the location of the dialog window was not retrieved, likely because it does not currently exist, or the dialogID is invalid.  The dialog window will exist anytime between the Setup message and OK/Cancel message.

## See Also
VS Functions:
[SetLayoutDialogPosition](SetLayoutDialogPosition.md)

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern


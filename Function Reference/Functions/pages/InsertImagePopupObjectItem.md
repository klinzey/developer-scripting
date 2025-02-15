# InsertImagePopupObjectItem

## Description
Inserts the specified object into the image popup.&lt;BR&gt;
&lt;BR&gt;
Note: the image popup only supports the following object types: gradients, hatches, images, record formats, render backgrounds, symbol folders, symbols, textures, vectorscript palettes, vectorscripts, worksheets.

```pascal
FUNCTION InsertImagePopupObjectItem(
				dialogID    : LONGINT;
				componentID : LONGINT;
				objectName  : STRING) : INTEGER;
```

```python

def vs.InsertImagePopupObjectItem(dialogID, componentID, objectName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|
|objectName|STRING|Name of the object to insert.|

## Returns
Returns an image popup index to the object inserted.

## Remarks
Functionality description needs more.

## Examples
```pascal
PROCEDURE dialog1_Main;

VAR

	dialog1 :INTEGER;

	int     :INTEGER;

	str     :STRING;



PROCEDURE dialog1_Handler(VAR item :LONGINT; data :LONGINT);

BEGIN

	CASE item OF

		SetupDialogC:

			BEGIN

				str := GetSDName(FSymDef);

				int := InsertImagePopupObjectItem(dialog1, 4, str);

				SetImagePopupSelectedItem(dialog1, 4, int);

			END;

	END;

END;



BEGIN

	dialog1 := CreateLayout('Image Pop-Up', FALSE, 'OK', '');

	CreateControl(dialog1, 4, 10, '', 0);

	SetFirstLayoutItem(dialog1, 4);

	int := RunLayoutDialog(dialog1, dialog1_Handler);

END;

RUN(dialog1_Main);


```

## See Also
VS Functions:
[GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObject](GetImagePopupObject.md)| [GetImagePopupObjectItemIndex](GetImagePopupObjectItemIndex.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [GetImagePopupSelectedItem](GetImagePopupSelectedItem.md)| [RemoveImagePopupItem](RemoveImagePopupItem.md)| [RemoveAllImagePopupItems](RemoveAllImagePopupItems.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


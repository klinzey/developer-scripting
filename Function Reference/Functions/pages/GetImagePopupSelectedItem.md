# GetImagePopupSelectedItem

## Description
Gets the selected image popup item.

```pascal
FUNCTION GetImagePopupSelectedItem(
				dialogID    : LONGINT;
				componentID : LONGINT) : INTEGER;
```

```python

def vs.GetImagePopupSelectedItem(dialogID, componentID):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|

## Returns
Returns the image popup index for the currently selected item.

## Examples
```pascal
selectedItemIndex := GetImagePopupSelectedItem(dialogID, componentID);
```

## See Also
VS Functions:
[InsertImagePopupObjectItem](InsertImagePopupObjectItem.md)| [GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObject](GetImagePopupObject.md)| [GetImagePopupObjectItemIndex](GetImagePopupObjectItemIndex.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [RemoveImagePopupItem](RemoveImagePopupItem.md)| [RemoveAllImagePopupItems](RemoveAllImagePopupItems.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


# RemoveImagePopupItem

## Description
Removes the specified item from the image popup.

```pascal
PROCEDURE RemoveImagePopupItem(
				dialogID    : LONGINT;
				componentID : LONGINT;
				itemIndex   : INTEGER);
```

```python

def vs.RemoveImagePopupItem(dialogID, componentID, itemIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|
|itemIndex|INTEGER|Index to item to be removed.|

## Examples
```pascal
RemoveImagePopupItem(dialogID, componentID, 4);
```

## See Also
VS Functions:
[InsertImagePopupObjectItem](InsertImagePopupObjectItem.md)| [GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObject](GetImagePopupObject.md)| [GetImagePopupObjectItemIndex](GetImagePopupObjectItemIndex.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [GetImagePopupSelectedItem](GetImagePopupSelectedItem.md)| [RemoveAllImagePopupItems](RemoveAllImagePopupItems.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


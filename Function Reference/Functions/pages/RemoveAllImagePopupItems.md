# RemoveAllImagePopupItems

## Description
Removes all items from the image popup.

```pascal
PROCEDURE RemoveAllImagePopupItems(
				dialogID    : LONGINT;
				componentID : LONGINT);
```

```python

def vs.RemoveAllImagePopupItems(dialogID, componentID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|

## Examples
```pascal
RemoveAllImagePopupItems(dialogID, componentID);
```

## See Also
VS Functions:
[InsertImagePopupObjectItem](InsertImagePopupObjectItem.md)| [GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObject](GetImagePopupObject.md)| [GetImagePopupObjectItemIndex](GetImagePopupObjectItemIndex.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [GetImagePopupSelectedItem](GetImagePopupSelectedItem.md)| [RemoveImagePopupItem](RemoveImagePopupItem.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


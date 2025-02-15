# GetImagePopupObject

## Description
Returns the object name for the specified image popup item.

```pascal
FUNCTION GetImagePopupObject(
				dialogID    : LONGINT;
				componentID : LONGINT;
				itemIndex   : INTEGER) : STRING;
```

```python

def vs.GetImagePopupObject(dialogID, componentID, itemIndex):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|
|itemIndex|INTEGER|Image popup item index for object to be retrieved.|

## Returns
Returns name of object stored at specified image popup index.

## Examples
```pascal
objectName := GetImagePopupObject(dialogID, componentID, 4);
```

## See Also
VS Functions:
[InsertImagePopupObjectItem](InsertImagePopupObjectItem.md)| [GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObjectItemIndex](GetImagePopupObjectItemIndex.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [GetImagePopupSelectedItem](GetImagePopupSelectedItem.md)| [RemoveImagePopupItem](RemoveImagePopupItem.md)| [RemoveAllImagePopupItems](RemoveAllImagePopupItems.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


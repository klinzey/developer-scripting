# GetImagePopupObjectItemIndex

## Description
Returns item index for the specified object.

```pascal
FUNCTION GetImagePopupObjectItemIndex(
				dialogID    : LONGINT;
				componentID : LONGINT;
				objectName  : STRING) : INTEGER;
```

```python

def vs.GetImagePopupObjectItemIndex(dialogID, componentID, objectName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|Index to a specific image popup component.|
|objectName|STRING|Name of object for which the image popup index should be retrieved.|

## Returns
Returns the image popup index for the specified object.

## Examples
```pascal
imagePopupIndex := GetImagePopupObjectItemIndex(dialogID, componentID, 'Symbol-1');
```

## See Also
VS Functions:
[InsertImagePopupObjectItem](InsertImagePopupObjectItem.md)| [GetNumImagePopupItems](GetNumImagePopupItems.md)| [GetImagePopupObject](GetImagePopupObject.md)| [SetImagePopupSelectedItem](SetImagePopupSelectedItem.md)| [GetImagePopupSelectedItem](GetImagePopupSelectedItem.md)| [RemoveImagePopupItem](RemoveImagePopupItem.md)| [RemoveAllImagePopupItems](RemoveAllImagePopupItems.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


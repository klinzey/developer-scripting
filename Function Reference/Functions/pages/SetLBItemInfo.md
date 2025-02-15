# SetLBItemInfo

## Description
Sets data for item.

```pascal
FUNCTION SetLBItemInfo(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				itemIndex    : INTEGER;
				subItemIndex : INTEGER;
				itemString   : STRING;
				imageIndex   : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBItemInfo(dialogID, componentID, itemIndex, subItemIndex, itemString, imageIndex):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|itemIndex|INTEGER|the item index|
|subItemIndex|INTEGER|the subitem index|
|itemString|STRING|the item text|
|imageIndex|INTEGER|the item image list index|

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


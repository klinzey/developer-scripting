# SetLBItemUsingColumnDataItem

## Description
Sets list item data with specified column data item.

```pascal
FUNCTION SetLBItemUsingColumnDataItem(
				dialogID            : LONGINT;
				componentID         : LONGINT;
				itemIndex           : INTEGER;
				subItemIndex        : INTEGER;
				columnDataItemIndex : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBItemUsingColumnDataItem(dialogID, componentID, itemIndex, subItemIndex, columnDataItemIndex):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|itemIndex|INTEGER|the row index|
|subItemIndex|INTEGER|the column index|
|columnDataItemIndex|INTEGER|the column data item with which to set list item data|

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


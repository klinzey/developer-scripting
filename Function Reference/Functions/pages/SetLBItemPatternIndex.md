# SetLBItemPatternIndex

## Description
Sets the specified list browser item's pattern index.

```pascal
FUNCTION SetLBItemPatternIndex(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				itemIndex    : INTEGER;
				subItemIndex : INTEGER;
				patIndex     : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBItemPatternIndex(dialogID, componentID, itemIndex, subItemIndex, patIndex):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|itemIndex|INTEGER|the row index|
|subItemIndex|INTEGER|the column index|
|patIndex|INTEGER|The pattern index of this item. Value from [1..71]|

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Modern - Browser


# SetLBColumnOwnerDrawnType

## Description
Sets the list browser column's owner drawn type.

```pascal
FUNCTION SetLBColumnOwnerDrawnType(
				dialogID       : LONGINT;
				componentID    : LONGINT;
				itemIndex      : INTEGER;
				subItemIndex   : INTEGER;
				ownerDrawnType : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBColumnOwnerDrawnType(dialogID, componentID, itemIndex, subItemIndex, ownerDrawnType):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|itemIndex|INTEGER|the row index|
|subItemIndex|INTEGER|the column index|
|ownerDrawnType|INTEGER|None - 0
Solid rect - 1
Dual solid rect - 2
Pattern rect - 3
Dual pattern rect - 4
Gradient or image - 5
Blank - 6
Text - 7
Dashed line - 8|

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern - Browser


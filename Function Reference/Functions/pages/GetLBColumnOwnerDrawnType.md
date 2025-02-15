# GetLBColumnOwnerDrawnType

## Description
Gets the list browser column's owner drawn type.

```pascal
FUNCTION GetLBColumnOwnerDrawnType(
				dialogID           : LONGINT;
				componentID        : LONGINT;
				itemIndex          : INTEGER;
				subItemIndex       : INTEGER;
				VAR ownerDrawnType : INTEGER) : BOOLEAN;
```

```python

def vs.GetLBColumnOwnerDrawnType(dialogID, componentID, itemIndex, subItemIndex):
    return (BOOLEAN, ownerDrawnType)
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


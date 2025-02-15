# GetLBItemDashStyle

## Description
Deprecated - will generate error. Use GetLBItemLineType instead.

```pascal
FUNCTION GetLBItemDashStyle(
				dialogID       : LONGINT;
				componentID    : LONGINT;
				itemIndex      : INTEGER;
				subItemIndex   : INTEGER;
				VAR styleIndex : INTEGER;
				VAR lineWeight : INTEGER) : BOOLEAN;
```

```python

def vs.GetLBItemDashStyle(dialogID, componentID, itemIndex, subItemIndex):
    return (BOOLEAN, styleIndex, lineWeight)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|itemIndex|INTEGER|the row index|
|subItemIndex|INTEGER|the column index|
|styleIndex|INTEGER|the dash line's style index|
|lineWeight|INTEGER|the dash line's line weight|

## Remarks
Deprecated - will generate error. Use GetLBItemLineType instead. The style index it used no longer exists. Line types are used instead. Original description was: Gets the specified list browser item's dash style.

## See Also
VS Functions:
[GetLBItemLineType](GetLBItemLineType.md)

## Version
```diff
- GetLBItemDashStyle is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern - Browser


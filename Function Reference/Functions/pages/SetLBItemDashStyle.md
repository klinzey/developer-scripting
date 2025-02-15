# SetLBItemDashStyle

## Description
Deprecated - will generate error. Use SetLBItemLineType instead.

```pascal
FUNCTION SetLBItemDashStyle(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				itemIndex    : INTEGER;
				subItemIndex : INTEGER;
				styleIndex   : INTEGER;
				lineWeight   : INTEGER) : BOOLEAN;
```

```python

def vs.SetLBItemDashStyle(dialogID, componentID, itemIndex, subItemIndex, styleIndex, lineWeight):
    return BOOLEAN
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
Deprecated - will generate error. Use SetLBItemLineType instead. The style index it used no longer exists. Line types are used instead. Original description was: Sets the specified list browser item's dash style.

## See Also
VS Functions:
[SetLBItemLineType](SetLBItemLineType.md)

## Version
```diff
- SetLBItemDashStyle is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern - Browser


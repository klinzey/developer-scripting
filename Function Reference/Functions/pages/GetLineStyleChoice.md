# GetLineStyleChoice

## Description
Deprecated - will generate error. Use GetLineTypeChoice instead.

```pascal
PROCEDURE GetLineStyleChoice(
				dialogID      : LONGINT;
				itemID        : LONGINT;
				VAR lineStyle : INTEGER);
```

```python

def vs.GetLineStyleChoice(dialogID, itemID):
    return lineStyle
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|lineStyle|INTEGER||

## Remarks
Deprecated - will generate error. Use GetLineTypeChoice instead. The linestyle it used to return was a dash list index that no longer exists. Line types are used instead. Original description was: Get current choice of line style popup dialog control.  Choice is an index into list of linestyles available in current document.

## See Also
VS Functions:
[GetLineTypeChoice](GetLineTypeChoice.md)

## Version
```diff
- GetLineStyleChoice is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


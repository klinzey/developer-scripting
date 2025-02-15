# SetLineStyleChoice

## Description
Deprecated - will generate error. Use SetLineTypeChoice instead.

```pascal
PROCEDURE SetLineStyleChoice(
				dialogID  : LONGINT;
				itemID    : LONGINT;
				lineStyle : INTEGER);
```

```python

def vs.SetLineStyleChoice(dialogID, itemID, lineStyle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|lineStyle|INTEGER||

## Remarks
The linestyle index no longer exists. Line types are used instead. Use SetLineTypeChoice instead. Original description was: Set the current choice of the line style popup dialog control to the specified index.

## See Also
VS Functions:
[SetLineTypeChoice](SetLineTypeChoice.md)

## Version
```diff
- SetLineStyleChoice is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


# SetLineAttributeData

## Description
Deprecated - will generate error. Use SetLineTypeAttriData instead.

```pascal
PROCEDURE SetLineAttributeData(
				dialogID   : LONGINT;
				itemID     : LONGINT;
				lineStyle  : INTEGER;
				lineWeight : INTEGER);
```

```python

def vs.SetLineAttributeData(dialogID, itemID, lineStyle, lineWeight):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|lineStyle|INTEGER||
|lineWeight|INTEGER||

## Remarks
Deprecated - will generate error. Use SetLineTypeAttriData instead. The linestyle it used to use was a dash list index that no longer exists. Line types are used instead. Original description was: The linestyle it used to use was a dash list index that no longer exists. Line types are used nstead.

## See Also
VS Functions:
[SetLineTypeAttriData](SetLineTypeAttriData.md)

## Version
```diff
- SetLineAttributeData is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


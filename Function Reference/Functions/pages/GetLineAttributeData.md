# GetLineAttributeData

## Description
Deprecated - will generate error. Use GetLineTypeAttriData instead.

```pascal
PROCEDURE GetLineAttributeData(
				dialogID       : LONGINT;
				itemID         : LONGINT;
				VAR lineStyle  : INTEGER;
				VAR lineWeight : INTEGER);
```

```python

def vs.GetLineAttributeData(dialogID, itemID):
    return (lineStyle, lineWeight)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT||
|itemID|LONGINT||
|lineStyle|INTEGER||
|lineWeight|INTEGER||

## Remarks
Deprecated - will generate error. Use GetLineTypeAttriData instead. The linestyle it used to return was a dash list index that no longer exists. Line types are used instead. Original description was: Get the current choices for the combined line style and line weight dialog control.  The line style value is an index and the line weight value is in mils. <BR>


## See Also
VS Functions:
[GetLineTypeAttriData](GetLineTypeAttriData.md)

## Version
```diff
- GetLineAttributeData is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


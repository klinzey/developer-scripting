# SetDLComponentPenStyles

## Description
Deprecated - will generate error. Use SetDLCompPenStylesN instead.

```pascal
FUNCTION SetDLComponentPenStyles(
				index         : INTEGER;
				penStyleLeft  : INTEGER;
				penStyleRight : INTEGER) : BOOLEAN;
```

```python

def vs.SetDLComponentPenStyles(index, penStyleLeft, penStyleRight):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|penStyleLeft|INTEGER|The pen style of the component's left line.  Positive values for patterns, negative values for dash styles.|
|penStyleRight|INTEGER|The pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use SetDLCompPenStylesN instead. The dash style it used no longer exists. Line types are used instead. Original description was: Sets the left and right pen styles for the component at index in the Double Line Preferences.

## See Also
VS Functions:
[SetDLCompPenStylesN](SetDLCompPenStylesN.md)

## Version
```diff
- SetDLComponentPenStyles is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.5
## Category
* Document Settings


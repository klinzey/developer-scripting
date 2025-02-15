# GetDLComponentPenStyles

## Description
Deprecated - will generate error. Use GetDLCompPenStylesN instead.

```pascal
FUNCTION GetDLComponentPenStyles(
				index             : INTEGER;
				VAR penStyleLeft  : INTEGER;
				VAR penStyleRight : INTEGER) : BOOLEAN;
```

```python

def vs.GetDLComponentPenStyles(index):
    return (BOOLEAN, penStyleLeft, penStyleRight)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|penStyleLeft|INTEGER|Returns the pen style of the component's left line.  Positive values for patters, negative values for dash styles.|
|penStyleRight|INTEGER|Returns the pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use GetDLCompPenStylesN instead. The dash style it used no longer exists. Line types are used instead. Original description was: Gets the left and right side pen styles of the component at index in the Double Line Preferences.

## See Also
VS Functions:
[GetDLCompPenStylesN](GetDLCompPenStylesN.md)

## Version
```diff
- GetDLComponentPenStyles is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.5
## Category
* Document Settings


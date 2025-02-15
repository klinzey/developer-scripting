# SetComponentPenStyles

## Description
Deprecated - will generate error. Use SetCompPenStylesN  instead.

```pascal
FUNCTION SetComponentPenStyles(
				object         : HANDLE;
				componentIndex : INTEGER;
				leftPenStyle   : INTEGER;
				rightPenStyle  : INTEGER) : BOOLEAN;
```

```python

def vs.SetComponentPenStyles(object, componentIndex, leftPenStyle, rightPenStyle):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|leftPenStyle|INTEGER|The pen style of the component's left line.  Positive values for patterns, negative values for dash styles.|
|rightPenStyle|INTEGER|The pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use SetCompPenStylesN  instead.The dash style it used no longer exists. Line types are used instead. Original description was: Sets the left and right pen styles for a component in an object.<BR>


## See Also
VS Functions:
[SetCompPenStylesN](SetCompPenStylesN.md)

## Version
```diff
- SetComponentPenStyles is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Objects - Architectural


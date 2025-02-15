# GetComponentPenStyles

## Description
Deprecated - will generate error. Use GetCompPenStylesN instead.

```pascal
FUNCTION GetComponentPenStyles(
				object            : HANDLE;
				componentIndex    : INTEGER;
				VAR leftPenStyle  : INTEGER;
				VAR rightPenStyle : INTEGER) : BOOLEAN;
```

```python

def vs.GetComponentPenStyles(object, componentIndex):
    return (BOOLEAN, leftPenStyle, rightPenStyle)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|leftPenStyle|INTEGER|Returns the pen style of the component's left line.  Positive values for patterns, negative values for dash styles.|
|rightPenStyle|INTEGER|Returns the pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use GetCompPenStylesN instead.The dash style it used no longer exists. Line types are used instead. Original description was: Gets the left and right side pen styles of a component in an object

## See Also
VS Functions:
[GetCompPenStylesN](GetCompPenStylesN.md)

## Version
```diff
- GetComponentPenStyles is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.0
## Category
* Objects - Architectural


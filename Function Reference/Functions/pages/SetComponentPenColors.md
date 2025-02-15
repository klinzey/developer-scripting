# SetComponentPenColors

## Description
Sets the colors of the pens of a component in an object.

```pascal
FUNCTION SetComponentPenColors(
				object            : HANDLE;
				componentIndex    : INTEGER;
				leftPenForeColor  : INTEGER;
				leftPenBackColor  : INTEGER;
				rightPenForeColor : INTEGER;
				rightPenBackColor : INTEGER) : BOOLEAN;
```

```python

def vs.SetComponentPenColors(object, componentIndex, leftPenForeColor, leftPenBackColor, rightPenForeColor, rightPenBackColor):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|leftPenForeColor|INTEGER|The fore color of the left pen.|
|leftPenBackColor|INTEGER|The back color of the left pen.|
|rightPenForeColor|INTEGER|The fore color of the right pen.|
|rightPenBackColor|INTEGER|The back color of the right pen.|

## See Also
VS Functions:
[GetComponentPenColors](GetComponentPenColors.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


# SetComponentFillColors

## Description
Sets the fore and back fill colors of a component in an object.

```pascal
FUNCTION SetComponentFillColors(
				object         : HANDLE;
				componentIndex : INTEGER;
				fillForeColor  : INTEGER;
				fillBackColor  : INTEGER) : BOOLEAN;
```

```python

def vs.SetComponentFillColors(object, componentIndex, fillForeColor, fillBackColor):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|fillForeColor|INTEGER|The fore color of the fill.|
|fillBackColor|INTEGER|The back color of the fill.|

## See Also
VS Functions:
[GetComponentFillColors](GetComponentFillColors.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


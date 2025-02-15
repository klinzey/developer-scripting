# GetComponentFillColors

## Description
Gets the fore and back fill colors of a component in an object.

```pascal
FUNCTION GetComponentFillColors(
				object            : HANDLE;
				componentIndex    : INTEGER;
				VAR fillForeColor : INTEGER;
				VAR fillBackColor : INTEGER) : BOOLEAN;
```

```python

def vs.GetComponentFillColors(object, componentIndex):
    return (BOOLEAN, fillForeColor, fillBackColor)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|fillForeColor|INTEGER|Returns the fore color of the fill.|
|fillBackColor|INTEGER|Returns the back color of the fill.|

## See Also
VS Functions:
[SetComponentFillColors](SetComponentFillColors.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


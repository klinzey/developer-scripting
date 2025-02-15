# SetComponentWidth

## Description
Sets the width of a component in an object.

```pascal
FUNCTION SetComponentWidth(
				object         : HANDLE;
				componentIndex : INTEGER;
				width          : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetComponentWidth(object, componentIndex, width):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|width|REAL (Coordinate)|The width of the component.|

## See Also
VS Functions:
[GetComponentWidth](GetComponentWidth.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


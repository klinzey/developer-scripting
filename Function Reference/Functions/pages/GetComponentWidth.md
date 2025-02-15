# GetComponentWidth

## Description
Gets the width of a component in an object.

```pascal
FUNCTION GetComponentWidth(
				object         : HANDLE;
				componentIndex : INTEGER;
				VAR width      : REAL) : BOOLEAN;
```

```python

def vs.GetComponentWidth(object, componentIndex):
    return (BOOLEAN, width)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|width|REAL|Returns the width of the component.|

## See Also
VS Functions:
[SetComponentWidth](SetComponentWidth.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


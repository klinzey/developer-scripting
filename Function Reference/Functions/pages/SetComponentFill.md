# SetComponentFill

## Description
Sets the fill of a component in an object.

```pascal
FUNCTION SetComponentFill(
				object         : HANDLE;
				componentIndex : INTEGER;
				fill           : LONGINT) : BOOLEAN;
```

```python

def vs.SetComponentFill(object, componentIndex, fill):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|fill|LONGINT|The fill of the component.  Positive values for patterns, negative object indexes for hatches.|

## See Also
VS Functions:
[GetComponentFill](GetComponentFill.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


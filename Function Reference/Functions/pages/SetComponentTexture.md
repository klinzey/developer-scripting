# SetComponentTexture

## Description
Sets the texture of a component in an object.

```pascal
FUNCTION SetComponentTexture(
				object         : HANDLE;
				componentIndex : INTEGER;
				texture        : LONGINT) : BOOLEAN;
```

```python

def vs.SetComponentTexture(object, componentIndex, texture):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|texture|LONGINT|The ref number of the texture. 0 for no texture. -1 for class texture.|

## See Also
VS Functions:
[GetComponentTexture](GetComponentTexture.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


# GetComponentTexture

## Description
Gets the texture of a component in an object.

```pascal
FUNCTION GetComponentTexture(
				object         : HANDLE;
				componentIndex : INTEGER;
				VAR texture    : LONGINT) : BOOLEAN;
```

```python

def vs.GetComponentTexture(object, componentIndex):
    return (BOOLEAN, texture)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|texture|LONGINT|Returns the ref number of the texture. 0 for no texture. -1 for class texture.|

## See Also
VS Functions:
[SetComponentTexture](SetComponentTexture.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


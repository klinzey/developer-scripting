# SetComponentClass

## Description
Sets the class of a component in an object.

```pascal
FUNCTION SetComponentClass(
				object         : HANDLE;
				componentIndex : INTEGER;
				componentClass : LONGINT) : BOOLEAN;
```

```python

def vs.SetComponentClass(object, componentIndex, componentClass):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|componentClass|LONGINT|The class of the component.|

## See Also
VS Functions:
[GetComponentClass](GetComponentClass.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


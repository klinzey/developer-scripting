# DeleteComponent

## Description
Deletes a component in an object.

```pascal
FUNCTION DeleteComponent(
				object         : HANDLE;
				componentIndex : INTEGER) : BOOLEAN;
```

```python

def vs.DeleteComponent(object, componentIndex):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component to delete.|

## See Also
VS Functions:
[InsertNewComponent](InsertNewComponent.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


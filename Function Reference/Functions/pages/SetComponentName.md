# SetComponentName

## Description
Sets the name of a component in an object.

```pascal
FUNCTION SetComponentName(
				object         : HANDLE;
				componentIndex : INTEGER;
				componentName  : STRING) : BOOLEAN;
```

```python

def vs.SetComponentName(object, componentIndex, componentName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|componentName|STRING|The name of the component.|

## See Also
VS Functions:
[GetComponentName](GetComponentName.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


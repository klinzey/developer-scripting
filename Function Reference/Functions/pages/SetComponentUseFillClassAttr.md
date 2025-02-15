# SetComponentUseFillClassAttr

## Description
Sets the use fill class attributes flag of a component in an object.

```pascal
FUNCTION SetComponentUseFillClassAttr(
				object                 : HANDLE;
				componentIndex         : INTEGER;
				useFillClassAttributes : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetComponentUseFillClassAttr(object, componentIndex, useFillClassAttributes):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|useFillClassAttributes|BOOLEAN|Whether or not the component will use class attributes for its fill.|

## See Also
VS Functions:
[GetComponentUseFillClassAttr](GetComponentUseFillClassAttr.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


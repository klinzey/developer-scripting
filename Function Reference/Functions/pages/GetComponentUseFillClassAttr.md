# GetComponentUseFillClassAttr

## Description
Gets the use fill class attributes flag of a component in an object.

```pascal
FUNCTION GetComponentUseFillClassAttr(
				object                     : HANDLE;
				componentIndex             : INTEGER;
				VAR useFillClassAttributes : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetComponentUseFillClassAttr(object, componentIndex):
    return (BOOLEAN, useFillClassAttributes)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|useFillClassAttributes|BOOLEAN|Returns whether or not the component is using class attributes for its fill.|

## See Also
VS Functions:
[SetComponentUseFillClassAttr](SetComponentUseFillClassAttr.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


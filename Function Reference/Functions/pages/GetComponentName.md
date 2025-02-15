# GetComponentName

## Description
Gets the name of a component in an object.

```pascal
FUNCTION GetComponentName(
				object         : HANDLE;
				componentIndex : INTEGER) : STRING;
```

```python

def vs.GetComponentName(object, componentIndex):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|

## Returns
The name of the component.

## See Also
VS Functions:
[SetComponentName](SetComponentName.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


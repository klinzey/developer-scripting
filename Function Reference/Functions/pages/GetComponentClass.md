# GetComponentClass

## Description
Gets the class of a component in an object.

```pascal
FUNCTION GetComponentClass(
				object             : HANDLE;
				componentIndex     : INTEGER;
				VAR componentClass : LONGINT) : BOOLEAN;
```

```python

def vs.GetComponentClass(object, componentIndex):
    return (BOOLEAN, componentClass)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|componentClass|LONGINT|Returns the class of the component.|

## See Also
VS Functions:
[SetComponentClass](SetComponentClass.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Architectural


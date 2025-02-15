# GetComponentNetVolume

## Description
Gets the net volume of a component in an object.

```pascal
FUNCTION GetComponentNetVolume(
				object         : HANDLE;
				componentIndex : INTEGER) : REAL;
```

```python

def vs.GetComponentNetVolume(object, componentIndex):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|

## Returns
The net volume of the component.

## See Also
VS Functions:
[GetComponentNetArea](GetComponentNetArea.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


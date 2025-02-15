# GetComponentNetArea

## Description
Gets the net area of a component in an object.

```pascal
FUNCTION GetComponentNetArea(
				object         : HANDLE;
				componentIndex : INTEGER) : REAL;
```

```python

def vs.GetComponentNetArea(object, componentIndex):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|

## Returns
The net area of the component.

## See Also
VS Functions:
[GetComponentNetVolume](GetComponentNetVolume.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


# SetComponentManualEdgeOffset

## Description
Sets the manual edge offset of a component in an object.

```pascal
FUNCTION SetComponentManualEdgeOffset(
				object           : HANDLE;
				componentIndex   : INTEGER;
				manualEdgeOffset : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetComponentManualEdgeOffset(object, componentIndex, manualEdgeOffset):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a  slab, Slab Style, or the Slab Preferences.|
|componentIndex|INTEGER|The index of the component.|
|manualEdgeOffset|REAL (Coordinate)|The manual edge offset.|

## See Also
VS Functions:
[GetComponentManualEdgeOffset](GetComponentManualEdgeOffset.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


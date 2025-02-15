# SetComponentPenWeights

## Description
Sets the left and right pen weights for a component in an object.

```pascal
FUNCTION SetComponentPenWeights(
				object         : HANDLE;
				componentIndex : INTEGER;
				leftPenWeight  : INTEGER;
				rightPenWeight : INTEGER) : BOOLEAN;
```

```python

def vs.SetComponentPenWeights(object, componentIndex, leftPenWeight, rightPenWeight):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|leftPenWeight|INTEGER|The pen weight of the component's left line.|
|rightPenWeight|INTEGER|The pen weight of the component's right line.|

## See Also
VS Functions:
[GetComponentPenWeights](GetComponentPenWeights.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


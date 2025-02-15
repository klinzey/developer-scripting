# GetComponentPenWeights

## Description
Gets the pen weights of the left and right sides of a component in an object.

```pascal
FUNCTION GetComponentPenWeights(
				object             : HANDLE;
				componentIndex     : INTEGER;
				VAR leftPenWeight  : INTEGER;
				VAR rightPenWeight : INTEGER) : BOOLEAN;
```

```python

def vs.GetComponentPenWeights(object, componentIndex):
    return (BOOLEAN, leftPenWeight, rightPenWeight)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|componentIndex|INTEGER|The index of the component.|
|leftPenWeight|INTEGER|Returns the pen weight of the component's left line.|
|rightPenWeight|INTEGER|Returns the pen weight of the component's right line.|

## See Also
VS Functions:
[SetComponentPenWeights](SetComponentPenWeights.md)

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


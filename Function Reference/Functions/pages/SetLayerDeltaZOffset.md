# SetLayerDeltaZOffset

## Description
Sets the wall height's offset to the layer delta z.

```pascal
FUNCTION SetLayerDeltaZOffset(
				theWall           : HANDLE;
				layerDeltaZOffset : REAL) : BOOLEAN;
```

```python

def vs.SetLayerDeltaZOffset(theWall, layerDeltaZOffset):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall.|
|layerDeltaZOffset|REAL|The wall height's offset to the layer delta z.|

## Returns
Returns success status.

## See Also
VS Functions:
[GetLayerDeltaZOffset](GetLayerDeltaZOffset.md)

## Version
```diff
- SetLayerDeltaZOffset is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.5
## Category
* Objects - Walls


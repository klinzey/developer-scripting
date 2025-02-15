# SetTexBitPaintNode

## Description
Procedure SetTexBitPaintNode sets the paint node of the referenced texture bitmap.

```pascal
PROCEDURE SetTexBitPaintNode(
				textureBitmap : HANDLE;
				paintNode     : HANDLE);
```

```python

def vs.SetTexBitPaintNode(textureBitmap, paintNode):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureBitmap|HANDLE|Handle to texture bitmap.|
|paintNode|HANDLE|Paint node for texture bitmap.|

## Remarks
Sets the texture bitmap's image paint node

## Version
```diff
- SetTexBitPaintNode is obsolete as of VectorWorks12.0
```

Availability: from VectorWorks8.0
## Category
* Textures


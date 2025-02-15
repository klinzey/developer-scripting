# GetTextureBitmap

## Description
Function GetTextureBitmap returns the bitmap object attached to the referenced texture.

```pascal
FUNCTION GetTextureBitmap(shaderRecord : HANDLE) : HANDLE;
```

```python

def vs.GetTextureBitmap(shaderRecord):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|shaderRecord|HANDLE|Handle to shader record.|

## Returns
 If there is no texture applied to an object the function returns NIL.

## Remarks
Returns the bitmap object attached to the shader record, NIL if none

## Version
Availability: from VectorWorks8.0
## Category
* Textures


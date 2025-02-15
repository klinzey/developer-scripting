# SetTextureRefN

## Description
Sets the texture reference for a specified object

```pascal
PROCEDURE SetTextureRefN(
				obj        : HANDLE;
				textureRef : LONGINT;
				texPartID  : LONGINT;
				texLayerID : LONGINT);
```

```python

def vs.SetTextureRefN(obj, textureRef, texPartID, texLayerID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE||
|textureRef|LONGINT||
|texPartID|LONGINT||
|texLayerID|LONGINT|0 for base, &gt;0 for decals|

## Version
Availability: from Vectorworks 2010
## Category
* Textures


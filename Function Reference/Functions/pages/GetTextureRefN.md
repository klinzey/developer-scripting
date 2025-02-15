# GetTextureRefN

## Description
Returns the texture reference for a specified object.

```pascal
FUNCTION GetTextureRefN(
				obj            : HANDLE;
				texPartID      : LONGINT;
				texLayerID     : LONGINT;
				resolveByClass : BOOLEAN) : LongInt;
```

```python

def vs.GetTextureRefN(obj, texPartID, texLayerID, resolveByClass):
    return LongInt
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE||
|texPartID|LONGINT||
|texLayerID|LONGINT|Texture layer ID, 0 for base, &gt;0 for decals|
|resolveByClass|BOOLEAN||

## Version
Availability: from Vectorworks 2010
## Category
* Textures


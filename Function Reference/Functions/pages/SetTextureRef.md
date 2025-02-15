# SetTextureRef

## Description
Function SetTextureRef sets the texture reference ID for the referenced object.

```pascal
PROCEDURE SetTextureRef(
				obj        : HANDLE;
				textureRef : LONGINT;
				partID     : INTEGER);
```

```python

def vs.SetTextureRef(obj, textureRef, partID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|textureRef|LONGINT|Texture reference ID.|
|partID|INTEGER|Part to be assigned texture reference.|

## Remarks
See GetTextureRef

## Version
```diff
- SetTextureRef is obsolete as of Vectorworks 2010
```

Availability: from VectorWorks8.0
## Category
* Textures


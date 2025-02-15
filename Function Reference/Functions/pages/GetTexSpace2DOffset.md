# GetTexSpace2DOffset

## Description
Procedure GetTexSpace2DOffset returns the 2D offset for the referenced texture space in real-world inches.

```pascal
PROCEDURE GetTexSpace2DOffset(
				textureSpace : HANDLE;
				VAR offsetU  : REAL;
				VAR offsetV  : REAL);
```

```python

def vs.GetTexSpace2DOffset(textureSpace):
    return (offsetU, offsetV)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|
|offsetU|REAL|Returns texture offset U component.|
|offsetV|REAL|returns texture offset V component.|

## Remarks
Gets the 2D offset for this texture space in real-world inches.

## Version
```diff
- GetTexSpace2DOffset is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures


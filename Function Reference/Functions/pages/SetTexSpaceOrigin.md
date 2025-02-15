# SetTexSpaceOrigin

## Description
Procedure SetTexSpaceOrigin sets the offset of the referenced texture space that takes coordinates from world space to texture space.

```pascal
PROCEDURE SetTexSpaceOrigin(
				textureSpace : HANDLE;
				offset       : REAL);
```

```python

def vs.SetTexSpaceOrigin(textureSpace, offset):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|
|offset|REAL|Texture space offset value.|

## Remarks
Sets the offset that takes coordinates from world space to texture space

## Version
```diff
- SetTexSpaceOrigin is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures


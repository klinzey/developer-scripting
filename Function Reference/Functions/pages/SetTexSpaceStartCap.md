# SetTexSpaceStartCap

## Description
Procedure SetTexSpaceStartCap sets the texture status of a referenced sweep or extrude. 

```pascal
PROCEDURE SetTexSpaceStartCap(
				textureSpace     : HANDLE;
				startCapTextured : BOOLEAN);
```

```python

def vs.SetTexSpaceStartCap(textureSpace, startCapTextured):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|
|startCapTextured|BOOLEAN|Texture start cap status.|

## Remarks
Sets whether start cap of extrude or sweep is textured

## Version
```diff
- SetTexSpaceStartCap is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures


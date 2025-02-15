# SetTexSpaceOrientU

## Description
Procedure SetTexSpaceOrientU specifies the vector that describes the u-axis of the referenced texture (from world space to texture space).

```pascal
PROCEDURE SetTexSpaceOrientU(
				textureSpace : HANDLE;
				uXAxis       : REAL;
				uYAxis       : REAL;
				uZAxis       : REAL);
```

```python

def vs.SetTexSpaceOrientU(textureSpace, uXAxis, uYAxis, uZAxis):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|
|uXAxis|REAL|Sets u-axis vector X component.|
|uYAxis|REAL|Sets u-axis vector Y component.|
|uZAxis|REAL|Sets u-axis vector Z component.|

## Remarks
Sets the u-axis for the texture space (from world space to texture space)

## Version
```diff
- SetTexSpaceOrientU is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures


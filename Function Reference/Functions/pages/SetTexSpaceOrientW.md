# SetTexSpaceOrientW

## Description
Procedure SetTexSpaceOrientW specifies the vector that describes the w-axis of the referenced texture (from world space to texture space).

```pascal
PROCEDURE SetTexSpaceOrientW(
				textureSpace : HANDLE;
				wXAxis       : REAL;
				wYAxis       : REAL;
				wZAxis       : REAL);
```

```python

def vs.SetTexSpaceOrientW(textureSpace, wXAxis, wYAxis, wZAxis):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|textureSpace|HANDLE|Handle to texture space.|
|wXAxis|REAL|Sets w-axis vector X component.|
|wYAxis|REAL|Sets w-axis vector Y component.|
|wZAxis|REAL|Sets w-axis vector Z component.|

## Remarks
Sets the w-axis for the texture space (from world space to texture space)

## Version
```diff
- SetTexSpaceOrientW is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures


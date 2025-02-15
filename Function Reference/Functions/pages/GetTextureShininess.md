# GetTextureShininess

## Description
Function GetTextureShininess returns the shininess value of the referenced texture. The value is expressed as a percentage value with 0 equaling &amp;quot;Dull&amp;quot;.

```pascal
FUNCTION GetTextureShininess(texture : HANDLE) : INTEGER;
```

```python

def vs.GetTextureShininess(texture):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|texture|HANDLE|Handle to texture.|

## Remarks
Percentage value - 0 equals 'Dull'

## Version
```diff
- GetTextureShininess is obsolete as of VectorWorks9.0
```

Availability: from VectorWorks8.0
## Category
* Textures


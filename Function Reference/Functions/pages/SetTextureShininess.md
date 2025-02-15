# SetTextureShininess

## Description
Procedure SetTextureShininess sets the shininess value of the referenced texture. The value is expressed as a percentage value in a range of 0-100 with 0 equaling &amp;quot;Dull&amp;quot;.&lt;BR&gt;


```pascal
PROCEDURE SetTextureShininess(
				texture   : HANDLE;
				shininess : INTEGER);
```

```python

def vs.SetTextureShininess(texture, shininess):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|texture|HANDLE|Handle to texture.|
|shininess|INTEGER|Shininess setting for texture.|

## Remarks
Percentage value - 0 equals dull

## Version
```diff
- SetTextureShininess is obsolete as of VectorWorks9.0
```

Availability: from VectorWorks8.0
## Category
* Textures


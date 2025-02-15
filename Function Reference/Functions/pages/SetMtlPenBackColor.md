# SetMtlPenBackColor

## Description
Deprecated - will generate error.

```pascal
PROCEDURE SetMtlPenBackColor(
				material : HANDLE;
				color    : LONGINT);
```

```python

def vs.SetMtlPenBackColor(material, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|material|HANDLE|Handle to material.|
|color|LONGINT|RGB color value.|

## Remarks
Deprecated - will generate error.

## Examples
```pascal
ColorIndexToRGB(214,cRed,cGrn,cBlu);

SetMtlPenBackColor(mtlHandle,cRed,cGrn,cBlu);
```

## Version
```diff
- SetMtlPenBackColor is obsolete as of Vectorworks 2022
```

Availability: from Vectorworks 2021
## Category
* Object Attributes


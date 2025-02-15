# SetMtlPenForeColor

## Description
Deprecated - will generate error.

```pascal
PROCEDURE SetMtlPenForeColor(
				material : HANDLE;
				color    : LONGINT);
```

```python

def vs.SetMtlPenForeColor(material, color):
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

SetMtlPenForeColor(mtlHandle,cRed,cGrn,cBlu);
```

## Version
```diff
- SetMtlPenForeColor is obsolete as of Vectorworks 2022
```

Availability: from Vectorworks 2021
## Category
* Object Attributes


# GetMtlPenForeColor

## Description
Deprecated - will generate error.

```pascal
PROCEDURE GetMtlPenForeColor(
				material  : HANDLE;
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.GetMtlPenForeColor(material):
    return (red, green, blue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|material|HANDLE|Handle to material.|
|red|LONGINT|Returns RGB color component (red).|
|green|LONGINT|Returns RGB color component (green).|
|blue|LONGINT|Returns RGB color component (blue).|

## Remarks
Deprecated - will generate error.

## Examples
```pascal
GetMtlPenForeColor(mtlHandle,cRed,cGrn,cBlu);

RGBToColorIndex(cRed,cGrn,cBlu,colorValue);
```

## Version
```diff
- GetMtlPenForeColor is obsolete as of Vectorworks 2022
```

Availability: from Vectorworks 2021
## Category
* Object Attributes


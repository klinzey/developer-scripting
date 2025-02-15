# GetPrefRGB

## Description
Procedure GetPrefRGB return the RGB color components of the specified preference item. The RGB values are in the range of 0 - 65535.

```pascal
PROCEDURE GetPrefRGB(
				prefIndex   : INTEGER;
				VAR colorRV : LONGINT;
				VAR colorGV : LONGINT;
				VAR colorBV : LONGINT);
```

```python

def vs.GetPrefRGB(prefIndex):
    return (colorRV, colorGV, colorBV)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item constant|
|colorRV|LONGINT|Returns RGB color component (red)|
|colorGV|LONGINT|Returns RGB color component (green)|
|colorBV|LONGINT|Returns RGB color component (blue)|

## See Also
VS Functions:
[SetPrefRGB](SetPrefRGB.md)

## Version
Availability: from Vectorworks 2009
## Category
* Document Settings


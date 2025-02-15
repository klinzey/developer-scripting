# GetClFillFore

## Description
Returns the fill foreground color setting of the specified class. The color is returned as the RGB components of the color. RGB values are in the range of 0~65535.&lt;BR&gt;


```pascal
PROCEDURE GetClFillFore(
				className   : STRING;
				VAR colorRV : LONGINT;
				VAR colorGV : LONGINT;
				VAR colorBV : LONGINT);
```

```python

def vs.GetClFillFore(className):
    return (colorRV, colorGV, colorBV)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|
|colorRV|LONGINT|Returns RGB color component (red).|
|colorGV|LONGINT|Returns RGB color component (green).|
|colorBV|LONGINT|Returns RGB color component (blue).|

## Remarks
Returns the fill foreground color setting of the class named className in parameters colorRV, colorGV, and colorBV.

## Examples
```pascal
GetClFillFore('Grassy Cover',cRed,cGrn,cBlu);

RGBToColorIndex(cRed,cGrn,cBlu,colorValue);


```

## Version
Availability: from VectorWorks8.0
## Category
* Classes


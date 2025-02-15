# SetClFillFore

## Description
Sets the fill foreground color of the specified class. The color must be specified using the RGB components of the desired color. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetClFillFore(
				className : STRING;
				color     : LONGINT);
```

```python

def vs.SetClFillFore(className, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|
|color|LONGINT|RGB color value.|

## Remarks
Changes the fill foreground color setting of the class named className.

## Examples
```pascal
ColorIndexToRGB(24,cRed,cGrn,cBlu);

SetClFillFore('Grassy Cover',cRed,cGrn,cBlu);
```

## Version
Availability: from VectorWorks8.0
## Category
* Classes


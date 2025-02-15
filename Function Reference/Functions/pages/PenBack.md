# PenBack

## Description
Procedure PenBack set the active pen background color for the document. RGB values are in the range of 0~65535.

```pascal
PROCEDURE PenBack(color : LONGINT);
```

```python

def vs.PenBack(color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|color|LONGINT|RGB color value to be set as active pen background.|

## Examples
```pascal
PenBack(65535,0,39321);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


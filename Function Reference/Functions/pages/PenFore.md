# PenFore

## Description
Procedure PenFore sets the active pen foreground color for the document. RGB values are in the range of 0~65535.

```pascal
PROCEDURE PenFore(color : LONGINT);
```

```python

def vs.PenFore(color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|color|LONGINT|RGB color value to be set as active pen foreground.|

## Examples
```pascal
PenFore(65535,0,39321);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


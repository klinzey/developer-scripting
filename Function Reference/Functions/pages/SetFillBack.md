# SetFillBack

## Description
Procedure SetFillBack sets the fill background color setting of the specified object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetFillBack(
				h     : HANDLE;
				color : LONGINT);
```

```python

def vs.SetFillBack(h, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|color|LONGINT|RGB color value.|

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Object Attributes


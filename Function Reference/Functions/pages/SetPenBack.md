# SetPenBack

## Description
Procedure SetPenBack sets the pen background color of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetPenBack(
				h     : HANDLE;
				color : LONGINT);
```

```python

def vs.SetPenBack(h, color):
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


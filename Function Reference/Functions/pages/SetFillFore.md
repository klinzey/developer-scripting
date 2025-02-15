# SetFillFore

## Description
Procedure SetFillFore sets the fill foreground color setting of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetFillFore(
				h     : HANDLE;
				color : LONGINT);
```

```python

def vs.SetFillFore(h, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|color|LONGINT|RGB color value.|

## Examples
```pascal
SetFillFore(h, 65535, 0, 0);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Object Attributes


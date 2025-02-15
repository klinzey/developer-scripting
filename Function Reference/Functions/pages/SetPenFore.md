# SetPenFore

## Description
Procedure SetPenFore sets the pen foreground color of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetPenFore(
				h     : HANDLE;
				color : LONGINT);
```

```python

def vs.SetPenFore(h, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|color|LONGINT|RGB color value.|

## Remarks
Be nice if it said what color values were legal. -JDW

## Examples
```pascal
SetPenFore(HandleToObj,65535,0,39321); 


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Object Attributes


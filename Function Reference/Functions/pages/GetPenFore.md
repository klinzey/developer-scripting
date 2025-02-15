# GetPenFore

## Description
Procedure GetPenFore returns the pen foreground color components of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE GetPenFore(
				h         : HANDLE;
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.GetPenFore(h):
    return (red, green, blue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|red|LONGINT|Returns RGB color component value.|
|green|LONGINT|Returns RGB color component value.|
|blue|LONGINT|Returns RGB color component value.|

## Examples
```pascal
GetPenFore(handleToObject,redValue,greenValue,blueValue);


```

## See Also
VS Functions:
[ColorIndexToRGB](ColorIndexToRGB.md)| [RGBToColorIndex](RGBToColorIndex.md)

## Version
Availability: from MiniCAD6.0
## Category
* Object Attributes


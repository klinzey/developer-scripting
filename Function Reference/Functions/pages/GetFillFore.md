# GetFillFore

## Description
Procedure GetFillFore returns the fill foreground color of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE GetFillFore(
				h         : HANDLE;
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.GetFillFore(h):
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
GetFillFore(handleToObject,redValue,greenValue,blueValue);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD6.0
## Category
* Object Attributes


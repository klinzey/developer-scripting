# FFillFore

## Description
Procedure FFillFore returns the current fill foreground color. RGB values are in the range of 0~65535.&lt;BR&gt;


```pascal
PROCEDURE FFillFore(
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.FFillFore():
    return (red, green, blue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|red|LONGINT|Returns RGB color component value.|
|green|LONGINT|Returns RGB color component value.|
|blue|LONGINT|Returns RGB color component value.|

## Examples
```pascal
FFillFore(redValue,greenValue,blueValue);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


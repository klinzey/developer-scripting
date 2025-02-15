# FFillBack

## Description
Procedure FFillBack returns the current fill background color. RGB values are in the range of 0~65535.&lt;BR&gt;


```pascal
PROCEDURE FFillBack(
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.FFillBack():
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
FFillBack(redValue,greenValue,blueValue);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


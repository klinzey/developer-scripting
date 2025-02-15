# GetPenBack

## Description
Procedure GetPenBack returns the pen background color of the referenced object. RGB values are in the range of 0~65535.

```pascal
PROCEDURE GetPenBack(
				h         : HANDLE;
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.GetPenBack(h):
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
PROCEDURE Example;

VAR

	h :HANDLE;

	r, g, b :LONGINT;

BEGIN

	h := FSActLayer;

	GetPenBack(h, r, g, b);

	Message('r= ', r, ' g= ', g, ' b= ', b);

END;

RUN(Example);
```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD6.0
## Category
* Object Attributes


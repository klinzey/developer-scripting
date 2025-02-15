# RGBToColorIndexN

## Description
Procedure RGBToColorIndexN converts the Vectorworks palette colors from its' red, green, and blue component values to the Vectorworks color index. Parameters red, green, and blue return the color components of the swatch, and parameter color is the Vectorworks color index. RGB values are in the range of 0~65535. Parameter ignoreBlackBackground specifies whether the black background preference should be ignored. If set to TRUE, black and white indexes will not be inverted in black background.&lt;BR&gt;
&lt;BR&gt;
A color table listing with associated index values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#colors&quot;&gt;Appendix&lt;/A&gt;.


```pascal
PROCEDURE RGBToColorIndexN(
				red                   : LONGINT;
				green                 : LONGINT;
				blue                  : LONGINT;
				VAR color             : INTEGER;
				ignoreBlackBackground : BOOLEAN);
```

```python

def vs.RGBToColorIndexN(red, green, blue, ignoreBlackBackground):
    return color
```

## Parameters
|Name|Type|Description|
|---|---|---|
|red|LONGINT|RGB color component value.|
|green|LONGINT|RGB color component value.|
|blue|LONGINT|RGB color component value.|
|color|INTEGER|Color index.|
|ignoreBlackBackground|BOOLEAN|Ignore black background preference setting or not.|

## Examples
```pascal
PROCEDURE Example;

VAR

	red, green, blue :LONGINT;

	colorIndex :INTEGER;

BEGIN

	GetPenFore(FSActLayer, red, green, blue);

	RGBToColorIndexN(red, green, blue, colorIndex, TRUE);

	Message(colorIndex);

END;

RUN(Example)
```

## Version
Availability: from Vectorworks 2010
## Category
* Utility


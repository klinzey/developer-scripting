# RGBToColorIndex

## Description
Procedure RGBToColorIndex converts the Vectorworks palette colors from its' red, green, and blue component values to the colors' palette position index. Parameters red, green, and blue return the color components of the swatch, and parameter color is the palette position ID of the color swatch. RGB values are in the range of 0~65535. &lt;BR&gt;
&lt;BR&gt;
A color table listing with associated index values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#colors&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE RGBToColorIndex(
				red       : LONGINT;
				green     : LONGINT;
				blue      : LONGINT;
				VAR color : INTEGER);
```

```python

def vs.RGBToColorIndex(red, green, blue):
    return color
```

## Parameters
|Name|Type|Description|
|---|---|---|
|red|LONGINT|RGB color component value.|
|green|LONGINT|RGB color component value.|
|blue|LONGINT|RGB color component value.|
|color|INTEGER|Color index.|

## Examples
```pascal
PROCEDURE Example;

VAR

	red, green, blue :LONGINT;

	colorIndex :INTEGER;

BEGIN

	GetPenFore(FSActLayer, red, green, blue);

	RGBToColorIndex(red, green, blue, colorIndex);

	Message(colorIndex);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD6.0
## Category
* Utility


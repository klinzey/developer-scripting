# ColorIndexToRGB

## Description
Procedure ColorIndexToRGB converts the Vectorworks palette colors from the colors' palette position index to its red, green, and blue component values. RGB values are in the range of 0~65535.&lt;BR&gt;
&lt;BR&gt;
A color table listing with associated index values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#colors&quot;&gt;Appendix&lt;/A&gt;.


```pascal
PROCEDURE ColorIndexToRGB(
				color     : INTEGER;
				VAR red   : LONGINT;
				VAR green : LONGINT;
				VAR blue  : LONGINT);
```

```python

def vs.ColorIndexToRGB(color):
    return (red, green, blue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|color|INTEGER|Color index.|
|red|LONGINT|RGB color component value.|
|green|LONGINT|RGB color component value.|
|blue|LONGINT|RGB color component value.|

## Examples
```pascal
ColorIndexToRGB(45,r,g,b);

{returns the color value components of the color at position 45}
```

## Version
Availability: from MiniCAD6.0
## Category
* Utility


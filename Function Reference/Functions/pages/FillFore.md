# FillFore

## Description
Procedure FillFore sets the active fill foreground color setting for the document. RGB values are in the range of 0~65535.&lt;BR&gt;


```pascal
PROCEDURE FillFore(color : LONGINT);
```

```python

def vs.FillFore(color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|color|LONGINT|RGB color value to set as active fill foreground color.|

## Examples
```pascal
FillFore(65535,0,39321);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


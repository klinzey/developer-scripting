# FillBack

## Description
Procedure FillBack sets the active fill background color setting for the document. RGB values are in the range of 0~65535.&lt;BR&gt;


```pascal
PROCEDURE FillBack(color : LONGINT);
```

```python

def vs.FillBack(color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|color|LONGINT|RGB color value to set as active fill background color.|

## Examples
```pascal
FillBack(65535,0,39321);


```

## See Also
VS Functions:
[RGBToColorIndex](RGBToColorIndex.md)| [ColorIndexToRGB](ColorIndexToRGB.md)

## Version
Availability: from MiniCAD
## Category
* Document Attributes


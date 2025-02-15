# SetClPenBack

## Description
Procedure SetClPenBack sets the pen background color of the specified class. The color must be specified using the RGB components of the desired color. RGB values are in the range of 0~65535.

```pascal
PROCEDURE SetClPenBack(
				className : STRING;
				color     : LONGINT);
```

```python

def vs.SetClPenBack(className, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|
|color|LONGINT|RGB color value.|

## Remarks
Changes the pen background color setting of the class named className.

## Examples
```pascal
ColorIndexToRGB(214,cRed,cGrn,cBlu);

SetClPenBack('Cold Water Supply',cRed,cGrn,cBlu);
```

## Version
Availability: from VectorWorks8.0
## Category
* Classes


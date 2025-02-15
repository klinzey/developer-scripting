# SetWSCellInsideVertBorder

## Description
Deprecated - use SetWsCellInsideVtBN instead

```pascal
PROCEDURE SetWSCellInsideVertBorder(
				worksheet   : HANDLE;
				topRow      : INTEGER;
				leftColumn  : INTEGER;
				bottomRow   : INTEGER;
				rightColumn : INTEGER;
				style       : INTEGER;
				weight      : INTEGER;
				color       : LONGINT);
```

```python

def vs.SetWSCellInsideVertBorder(worksheet, topRow, leftColumn, bottomRow, rightColumn, style, weight, color):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Worksheet on which function is to operate.|
|topRow|INTEGER|Top row of range to set.|
|leftColumn|INTEGER|Left column of range to set.|
|bottomRow|INTEGER|Bottom row of range to set.|
|rightColumn|INTEGER|Right column of range to set.|
|style|INTEGER|Border line style to be set.(0 = None; 2 = Solid, -1..-32 (dash style index) = Dash)|
|weight|INTEGER|Border line weight to be set.(in Mils)|
|color|LONGINT|Border line color to be set. (color index: 0..255)|

## Remarks
Deprecated - use SetWsCellInsideVtBN instead

## Version
```diff
- SetWSCellInsideVertBorder is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.5
## Category
* Worksheets


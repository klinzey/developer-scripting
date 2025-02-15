# SetWSCellBorder

## Description
Sets the borders of a cell in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
SetWSCellBorder allows text borders to be set for a rectangular range of cells. To set the border formatting of a single cell, specify identical values for the top/bottom and left/right range boundaries.&lt;BR&gt;


```pascal
PROCEDURE SetWSCellBorder(
				worksheet   : HANDLE;
				topRow      : INTEGER;
				leftColumn  : INTEGER;
				bottomRow   : INTEGER;
				rightColumn : INTEGER;
				top         : BOOLEAN;
				left        : BOOLEAN;
				bottom      : BOOLEAN;
				right       : BOOLEAN;
				outline     : BOOLEAN);
```

```python

def vs.SetWSCellBorder(worksheet, topRow, leftColumn, bottomRow, rightColumn, top, left, bottom, right, outline):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|topRow|INTEGER|Top row of cell range.|
|leftColumn|INTEGER|Leftmost column of cell range.|
|bottomRow|INTEGER|Bottom row of cell range.|
|rightColumn|INTEGER|Rightmost column of cell range.|
|top|BOOLEAN|Top border ON-OFF status.|
|left|BOOLEAN|Left border ON-OFF status.|
|bottom|BOOLEAN|Bottom border ON-OFF status.|
|right|BOOLEAN|Right border ON-OFF status.|
|outline|BOOLEAN|All borders ON-OFF status.|

## Remarks
OBSOLETE  for Version 12: see new SetWSCellBorders. [HOT 07/12/05]

## Version
```diff
- SetWSCellBorder is obsolete as of VectorWorks12.0
```

Availability: from VectorWorks9.0
## Category
* Worksheets


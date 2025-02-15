# SetWSCellVertAlignment

## Description
Sets the vertical alignment of cells in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
SetWSCellVertAlignment allows a vertical alignment to be set for a range of cells. To set the vertical alignment of a single cell, specify identical values for the top/bottom and left/right range boundaries.&lt;BR&gt;
&lt;BR&gt;
Note:&lt;BR&gt;
Vertical alignment constants:&lt;BR&gt;
top = 1&lt;BR&gt;
center  = 3&lt;BR&gt;
bottom = 5

```pascal
PROCEDURE SetWSCellVertAlignment(
				worksheet   : HANDLE;
				topRow      : INTEGER;
				leftColumn  : INTEGER;
				bottomRow   : INTEGER;
				rightColumn : INTEGER;
				vAlignment  : INTEGER);
```

```python

def vs.SetWSCellVertAlignment(worksheet, topRow, leftColumn, bottomRow, rightColumn, vAlignment):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet|
|topRow|INTEGER|Top row of cell range|
|leftColumn|INTEGER|Left column of cell range|
|bottomRow|INTEGER|Bottom row of cell range|
|rightColumn|INTEGER|Right column of cell range|
|vAlignment|INTEGER|Vertical alignment index value to be set|

## Remarks
Vertical alignment constants:<BR>
top = 1<BR>
center  = 3<BR>
bottom = 5

## Version
Availability: from VectorWorks12.0
## Category
* Worksheets


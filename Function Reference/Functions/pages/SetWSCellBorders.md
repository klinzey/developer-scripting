# SetWSCellBorders

## Description
Sets the borders of cells in the referenced worksheet&lt;BR&gt;
&lt;BR&gt;
SetWSCellBorders allows borders to be set for a rectangular range of cells. To set the border formatting of a single cell, specify identical values for the top/bottom and left/right range boundaries.&lt;BR&gt;
&lt;BR&gt;
Note:&lt;BR&gt;
A rectangular range of cells is formatted as a single block of cells. If you apply a right border to the range of cells, the border is displayed only on the right edge of the cells. &lt;BR&gt;
&lt;BR&gt;
The borders will be created with default values ( solid style, black color, standard weight).

```pascal
PROCEDURE SetWSCellBorders(
				worksheet     : HANDLE;
				topRow        : INTEGER;
				leftColumn    : INTEGER;
				bottomRow     : INTEGER;
				rightColumn   : INTEGER;
				top           : BOOLEAN;
				left          : BOOLEAN;
				bottom        : BOOLEAN;
				right         : BOOLEAN;
				OutlineInside : INTEGER);
```

```python

def vs.SetWSCellBorders(worksheet, topRow, leftColumn, bottomRow, rightColumn, top, left, bottom, right, OutlineInside):
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
|top|BOOLEAN|Top border ON-OFF status|
|left|BOOLEAN|Left border ON-OFF status|
|bottom|BOOLEAN|Bottom border ON-OFF status|
|right|BOOLEAN|Right border ON-OFF status|
|OutlineInside|INTEGER|Outline and Inside borders constant|

## Remarks
OulineInside defines the ouline, inside horizontal amd inside vertical borders.<BR>
Available constants:<BR>
0 : outline = false, inside horizontal = false,  inside vertical = false<BR>
1 : outline = true, inside horizontal = false,  inside vertical = false<BR>
2 : outline = false, inside horizontal = true,  inside vertical = false<BR>
3 : outline = true, inside horizontal = true,  inside vertical = false<BR>
4 : outline = false, inside horizontal = false,  inside vertical = true<BR>
5 : outline = true, inside horizontal = false,  inside vertical = true<BR>
6 : outline = false, inside horizontal = true,  inside vertical = true<BR>
7 : outline = true, inside horizontal = true,  inside vertical = true

## Examples
```pascal
{ Sets the inside horizontal and vertical borders for the specified rectangular range of cells}

SetWSCellBorders(sheet,2,4,1,5,FALSE,FALSE,FALSE,FALSE,6);



{ Sets an outline border for the specified rectangular range of cells}

SetWSCellBorders(sheet,2,4,1,5,FALSE,FALSE,FALSE,FALSE,1);

{or}

SetWSCellBorders(sheet,2,4,1,5,TRUE,TRUE,TRUE,TRUE,0);
```

## See Also
VS Functions:
[SetWSCellOutlineBorder](SetWSCellOutlineBorder.md)| [SetWSCellInsideVertBorder](SetWSCellInsideVertBorder.md)| [SetWSCellInsideHorizBorder](SetWSCellInsideHorizBorder.md)| [SetWSCellTopBorder](SetWSCellTopBorder.md)| [SetWSCellLeftBorder](SetWSCellLeftBorder.md)| [SetWSCellBottomBorder](SetWSCellBottomBorder.md)| [SetWSCellRightBorder](SetWSCellRightBorder.md)

## Version
Availability: from VectorWorks12.0
## Category
* Worksheets


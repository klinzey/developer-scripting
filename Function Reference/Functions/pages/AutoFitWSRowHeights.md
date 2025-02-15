# AutoFitWSRowHeights

## Description
Auto fit the height of rows to the content of the cells in the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
AutoFitWSRowHeights allows height for a range of rows to be auto fitted to the contents of cells. To auto fit the height of a single worksheet row, specify identical values for the top/bottom row range boundaries.

```pascal
PROCEDURE AutoFitWSRowHeights(
				worksheet : HANDLE;
				fromRow   : INTEGER;
				toRow     : INTEGER);
```

```python

def vs.AutoFitWSRowHeights(worksheet, fromRow, toRow):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet|
|fromRow|INTEGER|Top row of row range|
|toRow|INTEGER|Bottom row of row range|

## Examples
```pascal
{Auto resizes the height of all rows from row 1 to row 4} 

AutoFitWSRowHeights(sheet,1,4};
```

## Version
Availability: from VectorWorks12.0
## Category
* Worksheets


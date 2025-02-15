# SetWSCellFormula

## Description
Inserts a formula into a cell of the referenced worksheet.&lt;BR&gt;
&lt;BR&gt;
SetWSCellFormula allows a formula to be inserted into a rectangular range of cells. To insert a formula into a single cell, specify identical values for the top/bottom and left/right range boundaries.&lt;BR&gt;
&lt;BR&gt;
SetWSCellFormula triggers a worksheet recalculation if the AutoRecalc flag is set.&lt;BR&gt;
It is best to turn off that flag before using SetWSCellFormula repeatedly or in a loop and restore the flag after all operations are done (see GetWSAutoRecalcState and SetWSAutoRecalcState). &lt;BR&gt;
At the end, the worksheet should be recalculated by calling RecalculateWS.

```pascal
PROCEDURE SetWSCellFormula(
				worksheet   : HANDLE;
				topRow      : INTEGER;
				leftColumn  : INTEGER;
				bottomRow   : INTEGER;
				rightColumn : INTEGER;
				formula     : STRING);
```

```python

def vs.SetWSCellFormula(worksheet, topRow, leftColumn, bottomRow, rightColumn, formula):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|topRow|INTEGER|Top row of cell insertion range.|
|leftColumn|INTEGER|Leftmost column of cell insertion range.|
|bottomRow|INTEGER|Bottom row of cell insertion range.|
|rightColumn|INTEGER|Rightmost column of cell insertion range.|
|formula|STRING|Formula to be inserted into cell range.|

## Remarks
Sets specified formula string in specified worksheet cell(s).<BR>
If the 0 column is specified, a database row is created and the formula set as the database row criteria.

## Examples
```pascal
{ inserts a formula into a single cell }

SetWSCellFormula(h,4,2,4,2,'=3*2');



{ inserts a formula into a range of cells }

SetWSCellFormula(h,1,1,2,10,'&lt;empty&gt;');



{ creates a database sub-row for the record 'Part Info' }

SetWSCellFormula(h,2,0,2,0,'=DATABASE(R IN [''PART INFO''])');





///////////////////////////////////////////////////////////////



{Save the current AutoRecalc state}

state := GetWSAutoRecalcState(h);



{Turn off worksheet Auto Recalculation}

SetWSAutoRecalcState(h,false);



FOR i := 1 TO numCols DO

BEGIN

SetWSCellFormula (h, 1, i, 1, i, Num2Str (0, i));

SetWSCellFormula (h, 2, i, 2, i , Num2Str (0, i));

END;



{Restore AutoRecalc state}

SetWSAutoRecalcState(h, state);



{Now recalculate the worksheet}

RecalculateWS(h);


```

## See Also
VS Functions:
[GetWSAutoRecalcState](GetWSAutoRecalcState.md)| [SetWSAutoRecalcState](SetWSAutoRecalcState.md)

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


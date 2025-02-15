# GetWSCellString

## Description
Returns the displayed string value of a cell in the referenced worksheet.

```pascal
PROCEDURE GetWSCellString(
				worksheet      : HANDLE;
				row            : INTEGER;
				column         : INTEGER;
				VAR cellString : STRING);
```

```python

def vs.GetWSCellString(worksheet, row, column):
    return cellString
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|row|INTEGER|Row of cell to be queried.|
|column|INTEGER|Column of cell to be queried.|
|cellString|STRING|The string value contained in the worksheet cell.|

## Remarks
Gets the specified worksheet cell's displayed string.<BR>
If the cell contains a string, the displayed string IS that string.<BR>
If the cell contains a number, the displayed string is that number PLUS any formatting applied to that number.<BR>
Use IsWSCellString and/or MP_IsWSCellNumber to determine what type of value the cell actually contains. <BR>
Use GetWSCellValue to retrieve actual numerical value without  formatting from a cell that contains a number.

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


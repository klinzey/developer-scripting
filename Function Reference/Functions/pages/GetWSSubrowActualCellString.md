# GetWSSubrowActualCellString

## Description
Returns the actual string in a database subrow cell.

```pascal
PROCEDURE GetWSSubrowActualCellString(
				worksheet      : HANDLE;
				row            : INTEGER;
				column         : INTEGER;
				subrow         : INTEGER;
				VAR cellString : STRING);
```

```python

def vs.GetWSSubrowActualCellString(worksheet, row, column, subrow):
    return cellString
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|row|INTEGER|Database row to be queried.|
|column|INTEGER|Column to be queried.|
|subrow|INTEGER|Index of subrow cell to be queried.|
|cellString|STRING|Actual string of subrow cell.|

## Remarks
Gets the specified worksheet subrow cell's actual string.<BR>
WARNING: Because database subrow cells and their contents are dynamically created based on the current database of objects and the current critieria string any return values from this function are not guaranteed to be correct beyond this function call. Use this function carefully and at your own risk.

## Version
Availability: from VectorWorks 2008
## Category
* Worksheets


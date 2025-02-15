# RemoveWSColumnOperator

## Description
Removes database column operator from specified column.

```pascal
PROCEDURE RemoveWSColumnOperator(
				worksheet    : HANDLE;
				databaseRow  : INTEGER;
				column       : INTEGER;
				operatorType : INTEGER);
```

```python

def vs.RemoveWSColumnOperator(worksheet, databaseRow, column, operatorType):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|databaseRow|INTEGER|Database row to be queried.|
|column|INTEGER|Column to be queried.|
|operatorType|INTEGER|Operator type.|

## Remarks
Operator type constants:<BR>
All operators = -1<BR>
Sort operator = 0<BR>
Summarize operatory = 1

## Version
Availability: from Vectorworks 2012
## Category
* Worksheets


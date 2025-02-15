# IsWSDatabaseRow

## Description
Returns whether a row in the referenced worksheet is a database row.

```pascal
FUNCTION IsWSDatabaseRow(
				worksheet   : HANDLE;
				databaseRow : INTEGER) : BOOLEAN;
```

```python

def vs.IsWSDatabaseRow(worksheet, databaseRow):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|databaseRow|INTEGER|Row to be queried.|

## Returns
A BOOLEAN value indicating the database status of the targeted row.

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


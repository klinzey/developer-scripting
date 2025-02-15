# GetWSSubrowCount

## Description
Returns a count of displayed subrows for a specified database row.

```pascal
PROCEDURE GetWSSubrowCount(
				worksheet      : HANDLE;
				databaseRow    : INTEGER;
				VAR numSubrows : INTEGER);
```

```python

def vs.GetWSSubrowCount(worksheet, databaseRow):
    return numSubrows
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|databaseRow|INTEGER|Database row to be queried.|
|numSubrows|INTEGER|Number of displayed subrows.|

## Remarks
Gets the number of subrows associated with the specified worksheet database row.<BR>
WARNING: Because database subrow cells and their contents are dynamically created based on the current database of objects and the current critieria string any return values from this function are not guaranteed to be correct beyond this function call. Use this function carefully and at your own risk.

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


# GetWSSubrowHeight

## Description
Return the height of a database subrow in the referenced worksheet.

```pascal
PROCEDURE GetWSSubrowHeight(
				worksheet   : HANDLE;
				databaserow : INTEGER;
				subrow      : INTEGER;
				VAR height  : INTEGER);
```

```python

def vs.GetWSSubrowHeight(worksheet, databaserow, subrow):
    return height
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|databaserow|INTEGER|The database row|
|subrow|INTEGER|The database subrow to be queried|
|height|INTEGER|Output parameter. Return the height (in pixels)|

## Returns
Return the height of a database subrow in the referenced worksheet.

## Version
Availability: from Vectorworks 2009
## Category
* Worksheets


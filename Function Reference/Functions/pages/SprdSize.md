# SprdSize

## Description
Procedure SprdSize returns the number of rows and columns in the referenced worksheet.

```pascal
PROCEDURE SprdSize(
				h       : HANDLE;
				VAR row : INTEGER;
				VAR col : INTEGER);
```

```python

def vs.SprdSize(h):
    return (row, col)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|
|row|INTEGER|Returns row size of worksheet.|
|col|INTEGER|Returns column size of worksheet.|

## Remarks
OBSOLETE for Version 9: see new GetWSRowColumnCount. [VML 01/09/01]

## Version
```diff
- SprdSize is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


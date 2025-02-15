# GetCellNum

## Description
Function GetCellNum returns the numeric value of a cell in the referenced worksheet. 

```pascal
FUNCTION GetCellNum(
				h   : HANDLE;
				row : INTEGER;
				col : INTEGER) : REAL;
```

```python

def vs.GetCellNum(h, row, col):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|
|row|INTEGER|Worksheet row index.|
|col|INTEGER|Worksheet column index.|

## Remarks
OBSOLETE for Version 9: see new GetWSCellValue and GetWSSubrowCellValue. [VML 01/09/01]

## Version
```diff
- GetCellNum is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


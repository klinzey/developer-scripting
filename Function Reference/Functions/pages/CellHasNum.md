# CellHasNum

## Description
Function CellHasNum returns TRUE if the specified cell of a referenced worksheet contains a value or an equation which returns a numeric value.

```pascal
FUNCTION CellHasNum(
				h   : HANDLE;
				row : INTEGER;
				col : INTEGER) : BOOLEAN;
```

```python

def vs.CellHasNum(h, row, col):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|
|row|INTEGER|Worksheet row index.|
|col|INTEGER|Worksheet column index.|

## Remarks
OBSOLETE for Version 9: see new IsWSCellNumber and IsWSSubrowCellNumber. [VML 01/09/01]

## Version
```diff
- CellHasNum is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


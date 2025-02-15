# CellString

## Description
Function CellString returns the string of a specified cell in the active worksheet 

```pascal
FUNCTION CellString(
				row    : INTEGER;
				column : INTEGER) : STRING;
```

```python

def vs.CellString(row, column):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|row|INTEGER|Worksheet row index.|
|column|INTEGER|Worksheet column index.|

## Remarks
Returns the string representation of the current worksheet's cell specified by 'row' and 'column' numbers. [sd 8/13/98]<BR>
OBSOLETE for Version 9: see new GetWSCellString and GetWSSubrowCellString. [VML 01/09/01]

## Version
```diff
- CellString is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


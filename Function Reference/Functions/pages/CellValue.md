# CellValue

## Description
Function CellValue returns the numeric value of a specified cell in the active worksheet. If the specified cell is not a numeric type, then this function returns 0.&lt;BR&gt;


```pascal
FUNCTION CellValue(
				row    : INTEGER;
				column : INTEGER) : REAL;
```

```python

def vs.CellValue(row, column):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|row|INTEGER|Worksheet row index.|
|column|INTEGER|Worksheet column index.|

## Remarks
Returns the floating point representation of the current worksheet's cell specified by &quot;row&quot; and &quot;column&quot; numbers.  If the specified cell is not a numeric type, then this function returns 0. [sd 8/13/98]<BR>
OBSOLETE for Version 9: see new GetWSCellValue and GetWSSubrowCellValue. [VML 01/09/01]

## Version
```diff
- CellValue is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


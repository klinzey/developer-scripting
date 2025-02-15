# GetCellStr

## Description
Function GetCellStr returns the string value of a cell in the referenced worksheet. &lt;BR&gt;


```pascal
FUNCTION GetCellStr(
				h   : HANDLE;
				row : INTEGER;
				col : INTEGER) : STRING;
```

```python

def vs.GetCellStr(h, row, col):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|
|row|INTEGER|Worksheet row index.|
|col|INTEGER|Worksheet column index.|

## Remarks
OBSOLETE for Version 9: see new GetWSCellString and GetWSSubrowCellString. [VML 01/09/01]

## Version
```diff
- GetCellStr is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


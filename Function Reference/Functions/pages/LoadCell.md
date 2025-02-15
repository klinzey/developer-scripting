# LoadCell

## Description
Procedure LoadCell inserts a value into a specified cell of the active worksheet. 

```pascal
PROCEDURE LoadCell(
				ro    : INTEGER;
				col   : INTEGER;
				entry : STRING);
```

```python

def vs.LoadCell(ro, col, entry):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|ro|INTEGER|Worksheet row index.|
|col|INTEGER|Worksheet column index.|
|entry|STRING|Worksheet entry value.|

## Remarks
OBSOLETE for Version 9: see new SetWSCellFormula, SetWSCellBorder, SetWSCellAlignment, SetWSColumnWidth, SetWSCellTextFormat and SetWSCellNumberFormat. [VML 01/09/01]

## Examples
```pascal
SprdSheet(0,0,3,3);

LoadCell(1,1,'= (14 + 2) * 3');

{ inserts a formula into a cell }



SprdSheet(0,0,3,3);

LoadCell(1,1,'Window Schedule');

{ inserts a literal into a cell }




```

## Version
```diff
- LoadCell is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


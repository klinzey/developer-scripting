# GetCWidth

## Description
Function GetCWidth returns the column width of a cell in the referenced worksheet. &lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetCWidth(
				h   : HANDLE;
				row : INTEGER;
				col : INTEGER) : INTEGER;
```

```python

def vs.GetCWidth(h, row, col):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to worksheet.|
|row|INTEGER|Worksheet row index.|
|col|INTEGER|Worksheet column index.|

## Remarks
OBSOLETE for Version 9: see new GetWSColumnWidth. [VML 01/09/01]

## Version
```diff
- GetCWidth is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


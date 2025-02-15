# SprdWidth

## Description
Procedure SprdWidth specifies the width of cells in a worksheet when loaded.&lt;BR&gt;


```pascal
PROCEDURE SprdWidth(width : REAL);
```

```python

def vs.SprdWidth(width):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|width|REAL|Width of worksheet cell (0-255 characters).|

## Remarks
OBSOLETE for Version 9: see new SetWSColumnWidth. [VML 01/09/01]

## Examples
```pascal
SprdWidth(7);

LoadCell(1,1,'Cell 1,1');


```

## Version
```diff
- SprdWidth is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


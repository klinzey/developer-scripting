# SprdBorder

## Description
Procedure SprdBorder determines the border settings for cells within the active worksheet.&lt;BR&gt;


```pascal
PROCEDURE SprdBorder(
				top   : BOOLEAN;
				left  : BOOLEAN;
				bot   : BOOLEAN;
				right : BOOLEAN);
```

```python

def vs.SprdBorder(top, left, bot, right):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|top|BOOLEAN|Top border on-off setting.|
|left|BOOLEAN|Left border on-off setting.|
|bot|BOOLEAN|Bottom border on-off setting.|
|right|BOOLEAN|Right border on-off setting.|

## Remarks
OBSOLETE for Version 9: see new SetWSCellBorder. [VML 01/09/01]

## Examples
```pascal
SprdBorder(TRUE,FALSE,TRUE,FALSE);

LoadCell(1,1,'This is a string');


```

## Version
```diff
- SprdBorder is obsolete as of VectorWorks9.0
```

Availability: from MiniCAD
## Category
* Worksheets


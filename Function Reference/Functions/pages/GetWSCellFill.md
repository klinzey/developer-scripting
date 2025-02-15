# GetWSCellFill

## Description
Returns the fill style and color of a cell in the referenced worksheet

```pascal
PROCEDURE GetWSCellFill(
				worksheet       : HANDLE;
				row             : INTEGER;
				column          : INTEGER;
				VAR style       : INTEGER;
				VAR bgcolor     : LONGINT;
				VAR fgcolor     : LONGINT;
				VAR fillpattern : INTEGER);
```

```python

def vs.GetWSCellFill(worksheet, row, column):
    return (style, bgcolor, fgcolor, fillpattern)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet|
|row|INTEGER|Row of cell to be queried|
|column|INTEGER|Column of cell to be queried|
|style|INTEGER|Cell fill style constant|
|bgcolor|LONGINT|Cell background color index|
|fgcolor|LONGINT|Cell foreground color index|
|fillpattern|INTEGER|Cell pattern index|

## Remarks
bgcolor - cell background color  (0 if none)<BR>
fgcolor	- cell foreground color   (0 if none)<BR>
fillpattern - cell fill pattern index  (-1 if none)<BR>
<BR>
Fill style constants:<BR>
no fill = 0<BR>
solid fill= 1<BR>
pattern fill= 2

## Version
Availability: from VectorWorks12.0
## Category
* Worksheets


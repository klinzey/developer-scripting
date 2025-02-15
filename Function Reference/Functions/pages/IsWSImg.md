# IsWSImg

## Description
Determines if worksheet cell is set to display an image.

```pascal
FUNCTION IsWSImg(
				worksheet : HANDLE;
				row       : INTEGER;
				column    : INTEGER) : BOOLEAN;
```

```python

def vs.IsWSImg(worksheet, row, column):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|The worksheet handle.|
|row|INTEGER|The cell row.|
|column|INTEGER|The cell column.|

## Returns
A BOOLEAN value indicating whether the cell contains an image or not.

## Version
Availability: from Vectorworks 2014
## Category
* Worksheets


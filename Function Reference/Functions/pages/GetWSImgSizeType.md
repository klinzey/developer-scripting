# GetWSImgSizeType

## Description
Gets the worksheet cell's image size type.

```pascal
FUNCTION GetWSImgSizeType(
				worksheet : HANDLE;
				row       : INTEGER;
				column    : INTEGER) : INTEGER;
```

```python

def vs.GetWSImgSizeType(worksheet, row, column):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|The worksheet handle.|
|row|INTEGER|The cell row.|
|column|INTEGER|The cell column.|

## Returns
INTEGER specifying the cell image size type.

## Remarks
AutoSize size type = 0,<BR>
Fixed size type      = 1,<BR>
Scale size type     = 2

## Version
Availability: from Vectorworks 2014
## Category
* Worksheets


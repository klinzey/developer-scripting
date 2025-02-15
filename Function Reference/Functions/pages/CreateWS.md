# CreateWS

## Description
Creates a new worksheet in a Vectorworks document.

```pascal
FUNCTION CreateWS(
				name    : STRING;
				rows    : INTEGER;
				columns : INTEGER) : HANDLE;
```

```python

def vs.CreateWS(name, rows, columns):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|The name of the worksheet.|
|rows|INTEGER|The number of rows in the worksheet.|
|columns|INTEGER|The number of columns in the worksheet.|

## Returns
Returns a HANDLE to the new worksheet.

## Remarks
Creates a new worksheet object with the specified name and number of rows and columns.<BR>
If the name is in use, a legal available name based on the specified name will be used instead.<BR>
The number of rows must be &gt;= 1 and &lt;= 4094.<BR>
The number of columns must be &gt;= 1 and &lt;= 256.<BR>
NOTE: To create an on-drawing worksheet object, pass a worksheet handle to CreateWSImage.

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


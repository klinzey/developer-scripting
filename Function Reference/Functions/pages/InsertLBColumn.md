# InsertLBColumn

## Description
Inserts a column into the specified list browser control. Returns index of created column.

```pascal
FUNCTION InsertLBColumn(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				columnIndex  : INTEGER;
				headerString : STRING;
				width        : INTEGER) : INTEGER;
```

```python

def vs.InsertLBColumn(dialogID, componentID, columnIndex, headerString, width):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|columnIndex|INTEGER|index at which the column is to be inserted|
|headerString|STRING|text to set as column header|
|width|INTEGER|the width of the column in pixels|

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


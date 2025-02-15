# InsertLBColumnDataItem

## Description
Inserts column data item with specified data. Returns the index to the newly inserted item.

```pascal
FUNCTION InsertLBColumnDataItem(
				dialogID    : LONGINT;
				componentID : LONGINT;
				columnIndex : INTEGER;
				itemString  : STRING;
				imageOn     : INTEGER;
				imageOff    : INTEGER;
				itemData    : LONGINT) : INTEGER;
```

```python

def vs.InsertLBColumnDataItem(dialogID, componentID, columnIndex, itemString, imageOn, imageOff, itemData):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|columnIndex|INTEGER|the column for which to set the data|
|itemString|STRING|the item text|
|imageOn|INTEGER|the 'on' image list index|
|imageOff|INTEGER|the 'off' image list index|
|itemData|LONGINT|the item user data|

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


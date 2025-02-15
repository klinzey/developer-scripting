# GetLBEventInfo

## Description
Retrieves the last event information for the specified list browser.

```pascal
FUNCTION GetLBEventInfo(
				dialogID       : LONGINT;
				componentID    : LONGINT;
				VAR eventType  : INTEGER;
				VAR rowIndex   : INTEGER;
				VAR columIndex : INTEGER) : BOOLEAN;
```

```python

def vs.GetLBEventInfo(dialogID, componentID):
    return (BOOLEAN, eventType, rowIndex, columIndex)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|
|eventType|INTEGER||
|rowIndex|INTEGER|the row index where the click occurred.|
|columIndex|INTEGER|the column index where the click occurred.|

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern - Browser


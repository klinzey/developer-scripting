# GetControlData

## Description
Returns information about the specified extended control item.

```pascal
PROCEDURE GetControlData(
				dialogID : LONGINT;
				itemID   : LONGINT;
				VAR data : LONGINT);
```

```python

def vs.GetControlData(dialogID, itemID):
    return data
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index of dialog layout containing the control item.|
|itemID|LONGINT|Index of the control item.|
|data|LONGINT|Current setting of the control.|

## Remarks
[DWD 1/20/00]

## Version
Availability: from VectorWorks8.5
## Category
* Dialogs - Modern


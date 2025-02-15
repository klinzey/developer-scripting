# SetControlData

## Description
Sets the data for the specified extended control item. &lt;BR&gt;
&lt;BR&gt;
In image controls, for example, this call can be used to set the ID of the image resource being displayed.&lt;BR&gt;
&lt;BR&gt;
This function can only be called from within the dialog event handler subroutine.

```pascal
PROCEDURE SetControlData(
				dialogID : LONGINT;
				itemID   : LONGINT;
				data     : LONGINT);
```

```python

def vs.SetControlData(dialogID, itemID, data):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog containing the control.|
|itemID|LONGINT|The index of the dialog control item.|
|data|LONGINT|New data for the control item.|

## Remarks
[DWD 1/20/00]

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


# SetFirstGroupItem

## Description
Places the first item of a layout group into the specified group box control item. The control is inserted in the top left corner of the group box, and all other controls in the group are placed relative to this item.

```pascal
PROCEDURE SetFirstGroupItem(
				dialogID    : LONGINT;
				groupID     : LONGINT;
				firstItemID : LONGINT);
```

```python

def vs.SetFirstGroupItem(dialogID, groupID, firstItemID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout being defined.|
|groupID|LONGINT|The index of the group box control accepting the first item.|
|firstItemID|LONGINT|The index of the control item to be placed in the group box.|

## Remarks
[DWD 1/20/00]

## Examples
```pascal
SetFirstLayoutItem(lEditID,4);



{inserts the first control in a group box}

SetFirstGroupItem(lEditID,4,5);

	

SetBelowItem(lEditID,4,6,0,0);

SetFirstGroupItem(lEditID,6,7);

SetBelowItem(lEditID,6,8,0,0);


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


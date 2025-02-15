# SetFirstLayoutItem

## Description
Initializes dialog control layout by placing the specified control item in the top left corner of the layout. All other controls in the layout are positioned relative to the control item placed with this function.

```pascal
PROCEDURE SetFirstLayoutItem(
				dialogID    : LONGINT;
				firstItemID : LONGINT);
```

```python

def vs.SetFirstLayoutItem(dialogID, firstItemID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|The index of the dialog layout being defined.|
|firstItemID|LONGINT|The index of the control item to be placed.|

## Remarks
[DWD 1/20/00]

## Examples
```pascal
{positions the first control in the dialog}

SetFirstLayoutItem(lEditID,4);



SetFirstGroupItem(lEditID,4,5);	

SetBelowItem(lEditID,4,6,0,0);

SetFirstGroupItem(lEditID,6,7);

SetBelowItem(lEditID,6,8,0,0);


```

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern


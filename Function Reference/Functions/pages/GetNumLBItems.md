# GetNumLBItems

## Description
Gets the number of items in the specified list browser control.

```pascal
FUNCTION GetNumLBItems(
				dialogID    : LONGINT;
				componentID : LONGINT) : INTEGER;
```

```python

def vs.GetNumLBItems(dialogID, componentID):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|id of the dialog that contains the list browser|
|componentID|LONGINT|id of the list browser control|

## Returns
Returns the number of items in the list browser. 

## Version
Availability: from VectorWorks11.0
## Category
* Dialogs - Modern - Browser


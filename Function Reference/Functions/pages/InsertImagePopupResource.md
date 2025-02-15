# InsertImagePopupResource

## Description
Inserts the indicated item of the specified resource list into the indicated image popup and returns the image popup index of the inserted item.

```pascal
FUNCTION InsertImagePopupResource(
				dialogID    : LONGINT;
				componentID : LONGINT;
				listID      : LONGINT;
				index       : LONGINT) : LONGINT;
```

```python

def vs.InsertImagePopupResource(dialogID, componentID, listID, index):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|index to the dialog layout that contains the image popup component.|
|componentID|LONGINT|index to a specific image popup component.|
|listID|LONGINT|an ID for a resource list created by the BuildResourceList function.|
|index|LONGINT|an index into the list.|

## Examples
```pascal
{ Add all items in the resource list to the image popup. }

for index:=1 to numItems do

   index := InsertImagePopupResource(dialogID, kImagePopupID, listID,   index);


```

## Version
Availability: from VectorWorks12.0
## Category
* Dialogs - Modern


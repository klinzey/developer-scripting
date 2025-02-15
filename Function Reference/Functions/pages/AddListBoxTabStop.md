# AddListBoxTabStop

## Description
Adds a tab stop to a Layout Manager list box.  The last parameter is the tab stop, in characters.  This function should be called in the dialog handler, as opposed to the dialog definition procedure.  This function will clear all data in the list control.

```pascal
PROCEDURE AddListBoxTabStop(
				dialogID : LONGINT;
				itemID   : LONGINT;
				tabStop  : INTEGER);
```

```python

def vs.AddListBoxTabStop(dialogID, itemID, tabStop):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|ID of the dialog|
|itemID|LONGINT|ID of the list box|
|tabStop|INTEGER|The tab stop, in characters|

## Remarks
The last parameter is the tab stop, in characters.  This function should be called in the dialog handler, as opposed to the dialog definition procedure.  This function will clear all data in the list control.

## See Also
VS Functions:
[RemoveListBoxTabStop](RemoveListBoxTabStop.md)

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern


# AddChoice

## Description
Adds an item to the component's choices.

```pascal
PROCEDURE AddChoice(
				dialogID    : LONGINT;
				componentID : LONGINT;
				choiceText  : STRING;
				itemIndex   : INTEGER);
```

```python

def vs.AddChoice(dialogID, componentID, choiceText, itemIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the dialog identifier given by CreateLayout or CreateResizableLayout|
|componentID|LONGINT|The identifier for the component that contains the choices.|
|choiceText|STRING|The text for the item that is about to be added.|
|itemIndex|INTEGER|The index after which the new item is to be added.|

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Modern


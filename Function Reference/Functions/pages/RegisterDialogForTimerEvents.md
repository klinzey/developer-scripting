# RegisterDialogForTimerEvents

## Description
Register the dialog so that it can receive events periodically using the given time delay. Using the command will make Vectorworks send the event 'DialogTimerEventMessageC' to the dialog handler on the specified time interval.

```pascal
PROCEDURE RegisterDialogForTimerEvents(
				dialogID                 : LONGINT;
				timerDelayInMilliseconds : LONGINT);
```

```python

def vs.RegisterDialogForTimerEvents(dialogID, timerDelayInMilliseconds):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|the dialog identifier given by CreateLayout or CreateResizableLayout|
|timerDelayInMilliseconds|LONGINT|The amount of time in milliseconds between each event DialogTimerEventMessageC that is going to be sent to the dialog handler function.|

## Version
Availability: from Vectorworks 2010
## Category
* Dialogs - Modern


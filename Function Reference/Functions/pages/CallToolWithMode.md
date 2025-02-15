# CallToolWithMode

## Description
Activates the specified Vectorworks tool for a single use with the specified tool mode. After the tool has been used Vectorworks will revert back to the previously active tool.

```pascal
PROCEDURE CallToolWithMode(
				toolIndex  : INTEGER;
				modeGroup  : LONGINT;
				modeButton : LONGINT);
```

```python

def vs.CallToolWithMode(toolIndex, modeGroup, modeButton):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|toolIndex|INTEGER|Vectorworks tool constant.|
|modeGroup|LONGINT|Index of the mode group|
|modeButton|LONGINT|Index of the button in the group.|

## Remarks
Changes the active tool to that specified by toolID. Waits until the user has executed the functionality of that tool, then switches back to the previously active tool &amp; returns.

## Version
Availability: from Vectorworks 2016
## Category
* Utility


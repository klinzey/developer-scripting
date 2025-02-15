# Hide

## Description
Changes the object visibility to &amp;quot;invisible&amp;quot; for objects matching the specified search criteria. Hidden objects can be made visible with Show or UnHideObjects commands. Affects only objects on visible layers and classes.

```pascal
PROCEDURE Hide(c : CRITERIA);
```

```python

def vs.Hide(c):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Remarks
Makes objects with the specified search criteria invisible if they are not already<BR>
<BR>
[sd 8/18/98]

## Examples
```pascal
Hide((C='Proposed Phase 2 Construction'));
```

## Version
Availability: from MiniCAD
## Category
* Criteria


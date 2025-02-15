# Show

## Description
Changes the object visibility to &amp;quot;visible&amp;quot; for objects matching the specified search criteria. This is for object visibilities that were hidden with Hide, HideSelectedObjects and ShowOnlySelected commands. The object will only become visible if it is also on a visible layer and class.

```pascal
PROCEDURE Show(c : CRITERIA);
```

```python

def vs.Show(c):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Remarks
Makes objects with the specified search criteria visible if they are not already.<BR>
<BR>
[sd 8/18/98]

## Examples
```pascal
Show((C='Proposed Phase 2 Construction'));
```

## Version
Availability: from MiniCAD
## Category
* Criteria


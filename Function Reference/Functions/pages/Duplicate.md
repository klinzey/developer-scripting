# Duplicate

## Description
Procedure Duplicate copies the currently selected objects and moves them the specified offset distance.

```pascal
PROCEDURE Duplicate(offset : REAL);
```

```python

def vs.Duplicate(offset):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|offset|REAL|Offset value.|

## Examples
```pascal
Rect(0,1,1,0);

Duplicate(2,0);

{duplicates the rectangle 2 units right of the original}
```

## Version
Availability: from MiniCAD
## Category
* Object Editing


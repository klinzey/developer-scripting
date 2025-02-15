# LeftBound

## Description
Returns the x-coordinate of the bounding box (top left corner) of an object matching the search criteria. If more than one object matches the search criteria, the function will return the left value of the last matching object found.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION LeftBound(c : CRITERIA) : REAL;
```

```python

def vs.LeftBound(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
LeftBValue:=LeftBound(N='MyRect');
```

## Version
```diff
- LeftBound is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


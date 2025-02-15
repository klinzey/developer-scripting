# BotBound

## Description
Returns the y-coordinate of the bounding box (bottom right corner) of an object matching the search criteria. If more than one object matches the search criteria, the function will return the bottom value of the last matching object found.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION BotBound(c : CRITERIA) : REAL;
```

```python

def vs.BotBound(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
BotBValue:=BotBound(N='MyRect');


```

## Version
```diff
- BotBound is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


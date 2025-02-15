# TopBound

## Description
Returns the y-coordinate of the bounding box (top left corner) of an object matching the search criteria. If more than one object matches the search criteria, the function will return the sum of the coordinates of all the matching objects.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION TopBound(c : CRITERIA) : REAL;
```

```python

def vs.TopBound(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
TopBValue:=TopBound(N='MyRect');
```

## Version
```diff
- TopBound is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


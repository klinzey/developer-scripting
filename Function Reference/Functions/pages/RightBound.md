# RightBound

## Description
Returns the x-coordinate of the bounding box (bottom right corner) of an object matching the search criteria If more than one object matches the search criteria, the function will return the sum of the coordinates of all the matching objects.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION RightBound(c : CRITERIA) : REAL;
```

```python

def vs.RightBound(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
RightBValue:=RightBound(N='MyRect');


```

## Version
```diff
- RightBound is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


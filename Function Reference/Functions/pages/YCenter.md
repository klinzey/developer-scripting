# YCenter

## Description
Returns the y-coordinate of the center point of an object matching the serach criteria. If more than one object matches the search criteria, the function will return the sum of the coordinates of all the matching objects.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION YCenter(c : CRITERIA) : REAL;
```

```python

def vs.YCenter(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
YCenValue:=YCenter(N='Board');

{returns the y-coord of the center of the named object 'Board'}
```

## Version
```diff
- YCenter is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


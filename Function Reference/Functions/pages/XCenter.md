# XCenter

## Description
Returns the x-coordinate of the center point of an object matching the serach criteria. If more than one object matches the search criteria, the function will return the sum of the coordinates of all the matching objects.&lt;BR&gt;


```pascal
FUNCTION XCenter(c : CRITERIA) : REAL;
```

```python

def vs.XCenter(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
XCenValue:=XCenter(N='Board');

{returns the x-coord of the center of the named object 'Board'}
```

## Version
```diff
- XCenter is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


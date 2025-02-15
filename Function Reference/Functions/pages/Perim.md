# Perim

## Description
Returns the perimeter of an object. If more than one object matches the search criteria, the function will return the sum of the matching objects' perimeters.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Perim(c : CRITERIA) : REAL;
```

```python

def vs.Perim(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
PerimValue := Perim(C='Fence');

{returns the total perimeter of all objects in the class 'Fence'}
```

## Version
```diff
- Perim is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD
## Category
* Criteria


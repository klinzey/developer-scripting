# Area

## Description
Returns the area of an object. If more than one object matches the search criteria, the function will return the sum of all the matching object areas.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Area(c : CRITERIA) : REAL;
```

```python

def vs.Area(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Examples
```pascal
totalA:=Area((C='Plywood')and(L='First'));

{returns the area of all objects in class 'Plywood' on layer 'First'}
```

## Version
```diff
- Area is obsolete as of VectorWorks12.5
```

Availability: from MiniCAD
## Category
* Criteria


# CriteriaArea

## Description
Returns the area of an object. If more than one object matches the search criteria, the function will return the sum of all the matching object areas.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION CriteriaArea(c : CRITERIA) : REAL;
```

```python

def vs.CriteriaArea(c):
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
- CriteriaArea is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.0
## Category
* Criteria


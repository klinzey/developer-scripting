# Volume

## Description
Returns the volume of the items matching the specified criteria. If more than one object matches the search criteria, the sum of all the volumes of the matching objects will be returned. &lt;BR&gt;
&lt;BR&gt;
Volume will return only return volumes on objects which support the solids modelling functions.

```pascal
FUNCTION Volume(c : CRITERIA) : REAL;
```

```python

def vs.Volume(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Remarks
This function returns the volume of the items matching the current criteria.  It will return 0 for any objects that will not work with the solids modeling functions.

## Examples
```pascal
totalVol:=Volume((C='Empty Space'));
```

## Version
```diff
- Volume is obsolete as of VectorWorks12.5
```

Availability: from VectorWorks8.0
## Category
* Criteria


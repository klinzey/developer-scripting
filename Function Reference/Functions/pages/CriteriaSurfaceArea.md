# CriteriaSurfaceArea

## Description
Returns the surface area of the items matching the specified criteria. If more than one object matches the search criteria, the sum of all the surface areas of the matching objects will be returned. &lt;BR&gt;
&lt;BR&gt;
CriteriaSurfaceArea will return only return areas on objects which support the solids modelling functions.

```pascal
FUNCTION CriteriaSurfaceArea(c : CRITERIA) : REAL;
```

```python

def vs.CriteriaSurfaceArea(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Remarks
This function returns the surface area of the items matching the current criteria.  It will return 0 for any objects that will not work with the solids modeling functions.

## Examples
```pascal
totalArea:=CriteriaSurfaceArea((C='Empty Space'));
```

## Version
```diff
- CriteriaSurfaceArea is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.0
## Category
* Criteria


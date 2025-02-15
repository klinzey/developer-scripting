# SurfaceArea

## Description
Returns the surface area of the items matching the specified criteria. If more than one object matches the search criteria, the sum of all the surface areas of the matching objects will be returned. &lt;BR&gt;
&lt;BR&gt;
SurfaceArea will return only return areas on objects which support the solids modelling functions.

```pascal
FUNCTION SurfaceArea(c : CRITERIA) : REAL;
```

```python

def vs.SurfaceArea(c):
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
totalArea:=SurfaceArea((C='Empty Space'));
```

## Version
```diff
- SurfaceArea is obsolete as of VectorWorks12.5
```

Availability: from VectorWorks8.0
## Category
* Criteria


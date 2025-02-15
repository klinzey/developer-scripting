# CriteriaVolume

## Description
Returns the volume of the items matching the specified criteria. If more than one object matches the search criteria, the sum of all the volumes of the matching objects will be returned. &lt;BR&gt;
&lt;BR&gt;
CriteriaVolume will return only return volumes on objects which support the solids modelling functions.

```pascal
FUNCTION CriteriaVolume(c : CRITERIA) : REAL;
```

```python

def vs.CriteriaVolume(c):
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
totalVol:=CriteriaVolume((C='Empty Space'));
```

## Version
```diff
- CriteriaVolume is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.0
## Category
* Criteria


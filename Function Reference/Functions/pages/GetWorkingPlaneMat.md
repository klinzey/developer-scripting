# GetWorkingPlaneMat

## Description
Get the specified working plane matrix.

```pascal
PROCEDURE GetWorkingPlaneMat(
				refID           : LONGINT;
				VAR outCenterPt : REAL;
				VAR outNormal   : REAL;
				VAR outUVec     : REAL);
```

```python

def vs.GetWorkingPlaneMat(refID):
    return (outCenterPt, outNormal, outUVec)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|refID|LONGINT|Reference ID of the working plane.|
|outCenterPt|REAL|Output. The working plane center.|
|outNormal|REAL|Output. The working plane normal.|
|outUVec|REAL|Output. The U Vector of the plane.|

## Version
Availability: from Vectorworks 2011
## Category
* Utility


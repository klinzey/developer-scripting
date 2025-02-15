# SetCustomObjectWallHoleGroup

## Description
Set wall hole geometry for a parametric object.

```pascal
FUNCTION SetCustomObjectWallHoleGroup(
				objectHand : HANDLE;
				holeGroup  : HANDLE) : BOOLEAN;
```

```python

def vs.SetCustomObjectWallHoleGroup(objectHand, holeGroup):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHand|HANDLE|Handle to parametric object.|
|holeGroup|HANDLE|Handle to object or group that contains geometry for wall hole.|

## Returns
Returns TRUE if the operation was successful.

## Version
Availability: from Vectorworks 2009
## Category
* Objects - Custom


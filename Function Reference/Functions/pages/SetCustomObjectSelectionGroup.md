# SetCustomObjectSelectionGroup

## Description
Set selection indication geometry for a parametric object.

```pascal
FUNCTION SetCustomObjectSelectionGroup(
				objectHand : HANDLE;
				selGroup   : HANDLE) : BOOLEAN;
```

```python

def vs.SetCustomObjectSelectionGroup(objectHand, selGroup):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHand|HANDLE|Handle to parametric object.|
|selGroup|HANDLE|Handle to object or group that contains geometry for selection indication.|

## Returns
Returns TRUE if the operation was successful.

## Version
Availability: from Vectorworks 2009
## Category
* Objects - Custom


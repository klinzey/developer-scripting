# GetWallClosureGroup

## Description
Returns the handle to the wall closure group of an object.

```pascal
FUNCTION GetWallClosureGroup(hObjecct : HANDLE) : HANDLE;
```

```python

def vs.GetWallClosureGroup(hObjecct):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObjecct|HANDLE|Handlel to the object containing the wall closure group|

## Returns
The handle to an object's wall closure group. The handle will be NIL if no object is found.

## See Also
VS Functions:
[SetWallClosureGroup](SetWallClosureGroup.md)

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom


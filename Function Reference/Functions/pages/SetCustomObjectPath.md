# SetCustomObjectPath

## Description
Replaces the path of an existing path plug-in object.  The path is used as-is; no translation of vertices is performed.

```pascal
FUNCTION SetCustomObjectPath(
				objectHand : HANDLE;
				path       : HANDLE) : BOOLEAN;
```

```python

def vs.SetCustomObjectPath(objectHand, path):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHand|HANDLE|Handle to object.|
|path|HANDLE|Handle to new path polygon.|

## Returns
Returns TRUE if the operation was successful.

## See Also
VS Functions:
[GetCustomObjectPath](GetCustomObjectPath.md)

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Custom


# GetParent

## Description
Returns a handle to the parent container object of the referenced object. If the object does not have a container, a handle to the objects' layer will be returned.

```pascal
FUNCTION GetParent(h : HANDLE) : HANDLE;
```

```python

def vs.GetParent(h):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Returns
Returns a HANDLE to the parent object or layer.

## Version
Availability: from VectorWorks8.5
## Category
* Object Info


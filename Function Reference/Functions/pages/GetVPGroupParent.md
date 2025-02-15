# GetVPGroupParent

## Description
Gets the viewport that is the parent of specified viewport group.

```pascal
FUNCTION GetVPGroupParent(groupHandle : HANDLE) : HANDLE;
```

```python

def vs.GetVPGroupParent(groupHandle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|groupHandle|HANDLE|handle to a viewport group (crop, annotation, etc)|

## Returns
Returns a handle to the viewport object (type 122) that is the parent of the specified group, or nil if unsuccessful. 

## Version
Availability: from VectorWorks11.0
## Category
* Objects - Groups


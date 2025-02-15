# DTM6_IsObjectReady

## Description
Check if the DTM object is ready to be used. If this returns false, you should call 'ResetObject' on the handle to let the DTM object prepare itself to be used.

```pascal
FUNCTION DTM6_IsObjectReady(hDTMObject : HANDLE) : BOOLEAN;
```

```python

def vs.DTM6_IsObjectReady(hDTMObject):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hDTMObject|HANDLE||

## Version
Availability: from Vectorworks 2011
## Category
* SiteModel Interface Library


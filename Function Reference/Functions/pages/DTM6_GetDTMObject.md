# DTM6_GetDTMObject

## Description
Gets the DTM. If it's only one on the document and/or on the passed layer return it. If there are many DTMs ask the user to pick up one.

```pascal
FUNCTION DTM6_GetDTMObject(
				hLayer       : HANDLE;
				bPickUpModel : BOOLEAN) : HANDLE;
```

```python

def vs.DTM6_GetDTMObject(hLayer, bPickUpModel):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hLayer|HANDLE||
|bPickUpModel|BOOLEAN||

## Version
Availability: from Vectorworks 2011
## Category
* SiteModel Interface Library


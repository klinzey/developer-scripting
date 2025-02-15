# UpdateThumbnailPreview

## Description
For a given Vectorworks resource (i.e. Hatch, Texture, Symbol/PIO, etc...), this function will create or update it's thumbnail preview. 

```pascal
FUNCTION UpdateThumbnailPreview(resourceHandle : HANDLE) : BOOLEAN;
```

```python

def vs.UpdateThumbnailPreview(resourceHandle):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|resourceHandle|HANDLE|Handle to the resource.|

## Returns
This function returns true if the operation was successful, false otherwise.

## Version
Availability: from VectorWorks11.0
## Category
* Object Attributes


# CreatePaintFromImage

## Description
Creates a paint node from an image resource.

```pascal
FUNCTION CreatePaintFromImage(image : HANDLE) : HANDLE;
```

```python

def vs.CreatePaintFromImage(image):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|image|HANDLE|Handle to the image resource from which a paint node is to be created.|

## Returns
Returns the handle to the newly created paint node.

## Examples
```pascal
paintHandle := CreatePaintFromImage(imageHandle);
```

## Version
Availability: from VectorWorks10.0
## Category
* Textures


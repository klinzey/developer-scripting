# CreateImageFromPaint

## Description
Creates an image resource from a paint node.

```pascal
FUNCTION CreateImageFromPaint(
				paint     : HANDLE;
				imageName : STRING) : HANDLE;
```

```python

def vs.CreateImageFromPaint(paint, imageName):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|paint|HANDLE|Handle to the paint node to be used to create the image resource.|
|imageName|STRING|User-specified name to be used to identify the newly created image resource.|

## Returns
Returns the handle to the newly create image resource if successful; nil otherwise.

## Examples
```pascal
imageHandle := CreateImageFromPaint(paintHandle, 'My Image');
```

## Version
Availability: from VectorWorks10.0
## Category
* Document Attributes


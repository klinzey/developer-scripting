# CreatePaintFromImgN

## Description
Creates a paint node from an image resource on the specified location and rotation.

```pascal
FUNCTION CreatePaintFromImgN(
				image  : HANDLE;
				locPt  : REAL;
				rotDeg : REAL) : HANDLE;
```

```python

def vs.CreatePaintFromImgN(image, locPt, rotDeg):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|image|HANDLE|Handle to the image resource from which a paint node is to be created.|
|locPt|REAL|Location of the new paint nodet.|
|rotDeg|REAL|Rotation of the paint node in degrees.|

## Version
Availability: from Vectorworks 2011
## Category
* Textures


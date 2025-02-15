# CreateWSImage

## Description
Creates an in-document image of the specified worksheet. The specified point location is the top left corner of the image object.

```pascal
FUNCTION CreateWSImage(
				worksheet : HANDLE;
				location  : REAL) : HANDLE;
```

```python

def vs.CreateWSImage(worksheet, location):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|worksheet|HANDLE|Handle to worksheet.|
|location|REAL|X-Y coordinate location of image object.|

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets


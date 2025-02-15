# Get2DPt

## Description
Returns the location of the specified vertex of a referenced object.

```pascal
PROCEDURE Get2DPt(
				obj     : HANDLE;
				index   : INTEGER;
				VAR loc : REAL);
```

```python

def vs.Get2DPt(obj, index):
    return loc
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|index|INTEGER|Index of vertex to be queried.|
|loc|REAL|Coordinates of 2D vertex  location.|

## Version
Availability: from VectorWorks8.5
## Category
* Object Info


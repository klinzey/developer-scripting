# NurbsDelVertex

## Description
Deletes a point in the referenced NURBS curve or surface.&lt;BR&gt;
&lt;BR&gt;
The index is zero based (0 to number of points - 1).

```pascal
PROCEDURE NurbsDelVertex(
				objectHd : HANDLE;
				index1   : LONGINT;
				index2   : LONGINT);
```

```python

def vs.NurbsDelVertex(objectHd, index1, index2):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to NURBS curve or surface.|
|index1|LONGINT|Index of point in NURBS curve, or U-index of a point in NURBS surface.|
|index2|LONGINT|V-index of point in NURBS surface.|

## Remarks
this function will work for both nurbs curves and nurbs surfaces.DelObject should be used to completely remove a NURBS curve or surface from the drawing. It deletes the index2 point of the index1 piece for nurbs curve or It deletes an entire index2 row (index1 = 1) or column (index1 = 0)of points

## Version
Availability: from VectorWorks9.0
## Category
* Objects - NURBS


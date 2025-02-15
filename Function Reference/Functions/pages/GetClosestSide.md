# GetClosestSide

## Description
Returns the indices of the vertices that define the side closest to the specified location.  &lt;BR&gt;
&lt;BR&gt;
GetClosestSide supports only 2D objects.  If the object is unsupported, -1 will be returned as the index values.

```pascal
PROCEDURE GetClosestSide(
				obj        : HANDLE;
				pt         : REAL;
				VAR index1 : INTEGER;
				VAR index2 : INTEGER);
```

```python

def vs.GetClosestSide(obj, pt):
    return (index1, index2)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|pt|REAL|Coordinates of location.|
|index1|INTEGER|Index of first vertex of closest side.|
|index2|INTEGER|Index of second vertex of closest side.|

## Version
Availability: from VectorWorks8.5
## Category
* Utility


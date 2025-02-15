# GetPolyPt3D

## Description
Procedure GetPolyPt3D returns the coordinates of the specified vertex of the referenced mesh, 3D polygon, or NURBS curve object.&lt;BR&gt;
&lt;BR&gt;
Error checking for valid index values must be provided by the programmer.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE GetPolyPt3D(
				objectHd : HANDLE;
				index    : INTEGER;
				VAR p    : REAL);
```

```python

def vs.GetPolyPt3D(objectHd, index):
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to 3D mesh or polygon.|
|index|INTEGER|Index of vertex (range of 0 to n-1).|
|p|REAL|Returns 3D coordinates of vertex.|

## Examples
```pascal
for i := 0 to (GetVertNum(thePoly) - 1) do

begin		

	GetPolyPt3D(thePoly, i, vertX, vertY, vertZ);

end;	


```

## Version
Availability: from MiniCAD7.0
## Category
* Objects - 3D


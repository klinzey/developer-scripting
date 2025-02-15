# GetPolyPt

## Description
Procedure GetPolyPt returns the coordinates of a specified vertex of the referenced object.

```pascal
PROCEDURE GetPolyPt(
				objectHd : HANDLE;
				index    : INTEGER;
				VAR p    : REAL);
```

```python

def vs.GetPolyPt(objectHd, index):
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHd|HANDLE|Handle to polygon.|
|index|INTEGER|Index of vertex (range of 1 to n).|
|p|REAL|Returns coordinates of vertex.|

## Examples
```pascal
for i := 1 to GetVertNum(thePoly) do

begin		

	GetPolyPt(thePoly, i, vertX, vertY);

end;	


```

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


# GetPolylineArcMaxRadius

## Description
Return a maximum radius of the specified vertex of type arc or radius of a polyline. &lt;BR&gt;


```pascal
FUNCTION GetPolylineArcMaxRadius(
				hPoly     : HANDLE;
				vertexNum : INTEGER) : REAL;
```

```python

def vs.GetPolylineArcMaxRadius(hPoly, vertexNum):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hPoly|HANDLE|Handle of the poliline|
|vertexNum|INTEGER|Index of vertex to be queried.|

## Returns
If the vertex type is not arc or radius it returns -1.

## See Also
VS Functions:
[GetPolylineVertex](GetPolylineVertex.md)| [SetPolylineVertex](SetPolylineVertex.md)

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Polys


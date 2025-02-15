# CreateExtrudeAlongPath

## Description
Creates a new path extrude object in the document.  The profile defines the shape of the cross-section, and is extruded along the path to generate the resulting object.&lt;BR&gt;
&lt;BR&gt;
The path argument must be a handle to a NURBS Curve object (type 111).  The profile argument must be a handle to an object of one of the following types: NURBS Curve, Polygon, Polyline, Arc, Rectangle, Rounded Rectangle, Line, Oval.&lt;BR&gt;


```pascal
FUNCTION CreateExtrudeAlongPath(
				pathHandle    : HANDLE;
				profileHandle : HANDLE) : HANDLE;
```

```python

def vs.CreateExtrudeAlongPath(pathHandle, profileHandle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|pathHandle|HANDLE|Handle to the path object.|
|profileHandle|HANDLE|Handle to the profile object.|

## Returns
Returns a HANDLE to the new path extrude if successful, otherwise returns NIL.

## Remarks
The following objects are supported as profile objects:<BR>
<BR>
Line               2<BR>
Box                3<BR>
Oval               4<BR>
Polygon         5<BR>
Arc                6<BR>
Freehand       8<BR>
R Rect           13<BR>
Polyline        21<BR>
3D Poly        25<BR>
NURBS Curve 111<BR>
<BR>
<BR>
<BR>


## See Also
VS Functions:
[ExtrudeAlongPath](ExtrudeAlongPath.md)

## Version
Availability: from VectorWorks9.0
## Category
* Objects - 3D


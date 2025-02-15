# Set3DRot

## Description
Procedure Set3DRot rotates the referenced 3D object about a specified 3D point.  It works with the following 3D objects: extrude, multiple extrude, sweep, mesh, 3D polygon, solid, CSG solid, group, symbol, plug-in object, NURBS curve, NURBS surface.&lt;BR&gt;
&lt;BR&gt;
&lt;DIV ALIGN = &quot;CENTER&quot;&gt;&lt;IMG SRC = &quot;../Graphics/3drotate.gif&quot; border = &quot;0&quot; &gt;&lt;/DIV&gt;&lt;BR&gt;
&lt;BR&gt;
The difference between Set3DRot and SetRot3D is that Set3DRot adds the specified rotation to the existing rotation of the object, whereas SetRot3D does not consider the existing rotation, and merely makes the object rotation match the specified values.

```pascal
PROCEDURE Set3DRot(
				h         : HANDLE;
				xAngle    : REAL;
				yAngle    : REAL;
				zAngle    : REAL;
				xDistance : REAL (Coordinate);
				yDistance : REAL (Coordinate);
				zDistance : REAL (Coordinate));
```

```python

def vs.Set3DRot(h, xAngle, yAngle, zAngle, xDistance, yDistance, zDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to 3D object.|
|xAngle|REAL|X axis rotation angle.|
|yAngle|REAL|Y axis rotation angle.|
|zAngle|REAL|Z axis rotation angle.|
|xDistance|REAL (Coordinate)|X coordinate of center of rotation.|
|yDistance|REAL (Coordinate)|Y coordinate of center of rotation.|
|zDistance|REAL (Coordinate)|Z coordinate of center of rotation.|

## Examples
```pascal
Set3DRot(hd,10d,30d,23d45',3,3,2);


```

## See Also
VS Functions:
[SetRot3D](SetRot3D.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


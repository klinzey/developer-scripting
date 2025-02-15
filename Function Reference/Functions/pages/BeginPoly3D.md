# BeginPoly3D

## Description
Procedure BeginPoly3D creates a 3D polygon in the Vectorworks document. This procedure is used with Add3DPt and EndPoly3D to create 3D polygons. Any calls to the Add3DPt procedure after BeginPoly3D will be included in the 3D polygon.

```pascal
PROCEDURE BeginPoly3D;
```

```python

def vs.BeginPoly3D():
    return None
```

## Examples
```pascal
BeginPoly3D;

  Add3DPt(0,0,0);

  Add3DPt(2,0,0);

  Add3DPt(2,2,0);

  Add3DPt(1,3,0);

  Add3DPt(0,2,0);

  Add3DPt(0,0,0);

EndPoly3D;




```

## See Also
VS Functions:
[Add3DPt](Add3DPt.md)| [EndPoly3D](EndPoly3D.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


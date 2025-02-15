# EndPoly3D

## Description
Procedure EndPoly3D completes the definition of a multiple extrude object within a Vectorworks document. On calling EndPoly3D, the object is created in the document from the preceding object creation calls.&lt;BR&gt;
&lt;BR&gt;
It is recommended to call ResetOrientation3D after 3D object creations in order to ensure that the new 3D objects will draw properly.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE EndPoly3D;
```

```python

def vs.EndPoly3D():
    return None
```

## Remarks
[sd 8/14/98]

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
[BeginPoly3D](BeginPoly3D.md)| [Add3DPt](Add3DPt.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


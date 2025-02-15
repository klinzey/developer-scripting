# Add3DPt

## Description
Procedure Add3DPt adds a vertex into a newly created 3D polygon.&lt;BR&gt;
&lt;BR&gt;
Calls to Add3DPt should be made between calls to BeginPoly3D, which initiates polygon creation, and EndPoly3D, which terminates polygon creation. A minimum of two vertices must be created to define a valid 3D polygon object, and calculations may be performed within the BeginPoly3D-EndPoly3D structure, providing additional options for vertex generation.

```pascal
PROCEDURE Add3DPt(p : REAL);
```

```python

def vs.Add3DPt(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Location of 3D vertex.|

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
[BeginPoly3D](BeginPoly3D.md)| [EndPoly3D](EndPoly3D.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


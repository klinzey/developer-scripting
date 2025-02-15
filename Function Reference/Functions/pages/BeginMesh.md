# BeginMesh

## Description
Procedure BeginMesh begins the efinition of a 3D mesh object in Vectorworks. Any 3D point or planar object call after BeginMesh will be included in the mesh object. &lt;BR&gt;
&lt;BR&gt;
A mesh object allows the user to select and manipulate each vertex within its wire-frame model.

```pascal
PROCEDURE BeginMesh;
```

```python

def vs.BeginMesh():
    return None
```

## Examples
```pascal
BeginMesh;

ClosePoly;

PenSize(1);

PenPat(2);

FillPat(0);

Poly3D(0',0',4'-0&quot;,4'-0&quot;,0',4'-0&quot;,4'-0&quot;,-4'-0&quot;,4'-0&quot;,0',-4'-0&quot;,4'-0&quot;);

Smooth(0);

Poly3D(0',0',0',4'-0&quot;,0',0',4'-0&quot;,-4'-0&quot;,0',0',-4'-0&quot;,0');

Smooth(0);

Poly3D(0',-4'-0&quot;,0',0',-4'-0&quot;,4'-0&quot;,0',0',4'-0&quot;,0',0',0');

Poly3D(4'-0&quot;,-4'-0&quot;,0',4'-0&quot;,-4'-0&quot;,4'-0&quot;,0',-4'-0&quot;,4'-0&quot;,0',-4'-0&quot;,0');

Poly3D(4'-0&quot;,0',0',4'-0&quot;,0',4'-0&quot;,4'-0&quot;,-4'-0&quot;,4'-0&quot;,4'-0&quot;,-4'-0&quot;,0');

Poly3D(0',0',0',0',0',4'-0&quot;,4'-0&quot;,0',4'-0&quot;,4'-0&quot;,0',0');

EndMesh;


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


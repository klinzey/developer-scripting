# EndMesh

## Description
Procedure EndMesh completes the definition of a mesh object within a Vectorworks document. On calling EndMesh, the mesh is created in the document from the preceding object creation calls.&lt;BR&gt;
&lt;BR&gt;
It is recommended to call ResetOrientation3D after 3D object creations in order to ensure that the new 3D objects will draw properly.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE EndMesh;
```

```python

def vs.EndMesh():
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


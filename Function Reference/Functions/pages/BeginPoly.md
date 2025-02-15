# BeginPoly

## Description
Procedures BeginPoly creates a new polygon or polyline object in a Vectorworks document. When used with vertex creation procedure calls, BeginPoly and EndPoly() define the polygon object on a vertex by vertex basis.&lt;BR&gt;
&lt;BR&gt;
A minimum of two vertices must be created, and calculations may be performed within the creation structure between vertex calls, thus allowing additional flexibility in object generation.Hidden edges may be created by using use MoveTo() or Move() between vertex calls.

```pascal
PROCEDURE BeginPoly;
```

```python

def vs.BeginPoly():
    return None
```

## Examples
```pascal





```

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


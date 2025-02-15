# ClosePoly

## Description
Procedures ClosePoly set the polygon creation mode for polygon objects created in VectorScript to closed. To turn this mode off, use Procedure OpenPoly; the two modes used in conjunction will act as a toggle for the feature.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE ClosePoly;
```

```python

def vs.ClosePoly():
    return None
```

## Examples
```pascal
ClosePoly;

Poly(0,0,1,1,1,-1);

{creates a closed 3 sided polygon}
```

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


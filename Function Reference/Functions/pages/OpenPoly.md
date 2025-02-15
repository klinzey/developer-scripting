# OpenPoly

## Description
Procedures OpenPoly set the polygon creation mode for polygon objects created in VectorScript to open. To turn this mode off, use Procedure ClosePoly; the two modes used in conjunction will act as a toggle for the feature.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE OpenPoly;
```

```python

def vs.OpenPoly():
    return None
```

## Examples
```pascal
OpenPoly;

Poly(0,0,1,1,1,-1);

{creates a open 3 sided polygon}
```

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


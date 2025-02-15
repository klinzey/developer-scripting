# AddPoint

## Description
Procedure AddPoint adds a vertex point to a newly created polygon. AddPoint is designed to be used with BeginPoly and EndPoly to define new polygon objects via VectorScript.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE AddPoint(p : REAL);
```

```python

def vs.AddPoint(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Coordinates of vertex.|

## Examples
```pascal
BeginPoly;

     AddPoint(0,0);

     AddPoint(2,0);

     AddPoint(2,2);

     AddPoint(1,3);

     AddPoint(0,2);

     AddPoint(0,0);

EndPoly;

{creates a polygon object}



BeginPoly;

     AddPoint(x,y);

     x := x + 1;

     y := y + 1;

     AddPoint(x,y);

     x:= x + 1;

     y := y - 1;

     AddPoint(x,y);

EndPoly;

{creates a polygon with vertices as calculated}
```

## Version
Availability: from MiniCAD
## Category
* Objects - Polys


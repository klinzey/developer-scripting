# Relative

## Description
Sets the point designation method for VectorScript procedure calls. &lt;BR&gt;
&lt;BR&gt;
When this mode is active, all points specified in procedure calls are assumed to be X-Y offsets from the current graphics pen location. For example, the point designation (0,2) will move the graphics pen two vertical units away from its present location.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Relative;
```

```python

def vs.Relative():
    return None
```

## Examples
```pascal
Relative;

ClosePoly;

Poly(0,0,1,1,1,2,2,2,2,0);


```

## Version
Availability: from MiniCAD
## Category
* Command


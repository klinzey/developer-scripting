# EndVectorFill

## Description
Procedure EndVectorFill ends the vector fill creation process. This procedure call must follow the BeginVectorFillN call and a variable number of AddVectorFillLayer calls.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE EndVectorFill;
```

```python

def vs.EndVectorFill():
    return None
```

## Remarks
Follows BeginVectorFill and a variable number AddVectorFillLayer calls.

## Examples
```pascal
BeginVectorFill('Sample Hatch',TRUE,FALSE,0);

AddVectorFillLayer(0,0,1,1,0.5,-0.5,0.5,1,255);

AddVectorFillLayer(0.5,0.5,-2,0,1,-1,0.5,1,1);

EndVectorFill;


```

## Version
Availability: from MiniCAD7.0.1
## Category
* Hatches / Vector Fills


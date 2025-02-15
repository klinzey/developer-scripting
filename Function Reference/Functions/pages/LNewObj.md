# LNewObj

## Description
Returns a handle to the last object created by a VectorScript function call during the current script execution.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION LNewObj : HANDLE;
```

```python

def vs.LNewObj():
    return HANDLE
```

## Returns
Returns a HANDLE to the most recently created object, otherwise returns NIL.

## Remarks
[As of 8.0.0b10]<BR>
<BR>
If the object has been deleted since it was created, this function returns NIL. It is recommended that you call LNewObj immediately after the function or procedure which created the object to avoid problems.

## Version
Availability: from MiniCAD
## Category
* Document List Handling


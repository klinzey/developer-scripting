# EndSweep

## Description
Procedure EndSweep completes the definition of a sweep object within a Vectorworks document. On calling EndSweep, the object is created in the document from the preceding object creation calls.&lt;BR&gt;
&lt;BR&gt;
It is recommended to call ResetOrientation3D after 3D object creations in order to ensure that the new 3D objects will draw properly.&lt;BR&gt;


```pascal
PROCEDURE EndSweep;
```

```python

def vs.EndSweep():
    return None
```

## Examples
```pascal
BeginSweep(#0°,#360°,#10°,0');

  Poly(3 1/4&quot;,-1/2&quot;,3 1/4&quot;,-1&quot;,2 3/4&quot;,-1&quot;,

  2 1/4&quot;,-1/2&quot;,2 1/4&quot;,1&quot;,1 3/4&quot;,1 1/2&quot;,

  -1 3/4&quot;,1 1/2&quot;,-2 1/4&quot;,1&quot;,-2 1/4&quot;,-1/2&quot;,

  -2 3/4&quot;,-1&quot;,-3 1/4&quot;,-1&quot;,-3 1/4&quot;,-1/2&quot;,

  -2 3/4&quot;,0&quot;,-2 3/4&quot;,1 1/2&quot;,-2 1/4&quot;,2&quot;,

  2 1/4&quot;,2&quot;,2 3/4&quot;,1 1/2&quot;,2 3/4&quot;,0&quot;);

EndSweep;




```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


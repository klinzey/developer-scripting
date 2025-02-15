# EndXtrd

## Description
Procedure EndXtrd completes the definition of an extrude object within a Vectorworks document. On calling EndXtrd, the object is created in the document from the preceding object creation calls.&lt;BR&gt;
&lt;BR&gt;
It is recommended to call ResetOrientation3D after 3D object creations in order to ensure that the new 3D objects will draw properly.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE EndXtrd;
```

```python

def vs.EndXtrd():
    return None
```

## Examples
```pascal
BeginXtrd(0',4');

 Rect(-1 61/64&quot;,125/128&quot;,-1 119/256&quot;,-375/512&quot;);

 Rect(-1 113/512&quot;,1 113/512&quot;,-375/512&quot;,-125/256&quot;);

 Rect(-125/256&quot;,125/128&quot;,0',-375/512&quot;);

 Rect(125/128&quot;,125/128&quot;,1 119/256&quot;,-375/512&quot;);

 Rect(1 25/512&quot;,1 113/512&quot;,375/512&quot;,-125/256&quot;);

 Rect(1 363/512&quot;,1 113/512&quot;,2 101/512&quot;,-125/256&quot;);

EndXtrd;


```

## Version
Availability: from MiniCAD
## Category
* Objects - 3D


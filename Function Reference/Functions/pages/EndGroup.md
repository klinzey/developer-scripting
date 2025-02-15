# EndGroup

## Description
Procedure EndGroup completes the creation of a new group object in a Vectorworks document. The new group object is then generated in the document.&lt;BR&gt;


```pascal
PROCEDURE EndGroup;
```

```python

def vs.EndGroup():
    return None
```

## Examples
```pascal
BeginGroup;

Rect(-1,1,0.5,0);

Rect(0,1.5,1,0.5);

Oval(-1.5,0.5,-0.5,-0.5);

EndGroup;

{creates a group object}



BeginGroup;

Rect(-1,1,0,0.5);

Rect(-1,0.5,-0.5,0);

BeginGroup;

Oval(-0.5,0.5,1,0);

Oval(0,0,1,-0.5);

EndGroup;

EndGroup;

{creates a group comprised of 2 rects and 1 group}
```

## Version
Availability: from MiniCAD
## Category
* Objects - Groups


# Group

## Description
Procedures Group groups selected objects in a Vectorworks document. Any selected objects on the active layer(or any selected objects in the document when in Show-Snap-Modify mode) will be included in the new group object.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Group;
```

```python

def vs.Group():
    return None
```

## Examples
```pascal
Rect(-1,1,0,0);

Rect(-1,-0.5,0,-1.5);

Group;

{groups the most recently created objects}






```

## Version
Availability: from MiniCAD
## Category
* Objects - Groups


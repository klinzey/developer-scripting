# DeleteObjs

## Description
Procedure DeleteObjs deletes all selected objects on the active layer. Using this procedure when the layer display mode is Show/Snap/Modify will cause selected objects on any visible layer will be deleted.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE DeleteObjs;
```

```python

def vs.DeleteObjs():
    return None
```

## Examples
```pascal
DSelectAll;

SelectObj(((T=Locus) &amp; (NOT V)));

DeleteObjs;


```

## Version
Availability: from MiniCAD
## Category
* Object Editing


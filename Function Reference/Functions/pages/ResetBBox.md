# ResetBBox

## Description
Procedure ResetBBox forces the bounding box information for the specified object to be recomputed based on the objects' current geometry. &lt;BR&gt;
&lt;BR&gt;
Call this procedure after modifying an object to force a redraw of the object.

```pascal
PROCEDURE ResetBBox(h : HANDLE);
```

```python

def vs.ResetBBox(h):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Remarks
Forces the bouding box information for object h to be recomputed based on current geometry.<BR>
<BR>
[sd 8/14/98]

## Version
Availability: from MiniCAD
## Category
* Object Editing


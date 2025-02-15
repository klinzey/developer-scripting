# GetBBox

## Description
Procedure GetBBox returns the bounding box coordinates of the projection of the referenced object on the screen plane. &lt;BR&gt;


```pascal
PROCEDURE GetBBox(
				h      : HANDLE;
				VAR p1 : REAL;
				VAR p2 : REAL);
```

```python

def vs.GetBBox(h):
    return (p1, p2)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|p1|REAL|Top left coordinate of bounding box.|
|p2|REAL|Bottom right coordinate of bounding box.|

## Version
Availability: from MiniCAD
## Category
* Object Info


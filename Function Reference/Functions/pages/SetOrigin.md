# SetOrigin

## Description
Shifts the position of the document origin. The function does not modify the relative &lt;BR&gt;
positions of objects in the document; the coordinate locations of objects, however, &lt;BR&gt;
will change when the origin location is modified.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetOrigin(
				x : REAL;
				y : REAL);
```

```python

def vs.SetOrigin(x, y):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|x|REAL|X-offset from current origin.|
|y|REAL|Y-offset from current origin.|

## Examples
```pascal
Rect(0,0,1,1);

SetOrigin(1,1);



{ Creates a rectangle with the bottom left point at coordinates (0,0), then moves the origin so that the top right point of the rectangle has coordinates (0,0). }
```

## See Also
VS Functions:
[SetOriginAbsolute](SetOriginAbsolute.md)

## Version
Availability: from MiniCAD
## Category
* Document Settings


# HMove

## Description
Procedure HMove moves the referenced object a relative offset distance.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE HMove(
				h       : HANDLE;
				xOffset : REAL;
				yOffset : REAL);
```

```python

def vs.HMove(h, xOffset, yOffset):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|xOffset|REAL|X offset distance.|
|yOffset|REAL|Y offset distance.|

## Examples
```pascal
HMove(handleToObject,2,2);


```

## Version
Availability: from MiniCAD
## Category
* Object Editing


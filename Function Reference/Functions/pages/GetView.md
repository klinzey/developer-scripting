# GetView

## Description
Returns information about the current 3D view.

```pascal
PROCEDURE GetView(
				VAR xAngleR : REAL;
				VAR yAngelR : REAL;
				VAR zAngleR : REAL;
				VAR offset  : REAL);
```

```python

def vs.GetView():
    return (xAngleR, yAngelR, zAngleR, offset)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|xAngleR|REAL|Returns X rotation angle of view.|
|yAngelR|REAL|Returns Y rotation angle of view.|
|zAngleR|REAL|Returns Z rotation angle of view.|
|offset|REAL|Center of view rotation.|

## Remarks
Returns information about the current 3D view.<BR>
All parameters are for output:<BR>
xAngleR, the angle the view is rotated away from the x-axis<BR>
yAngleR, the angle the view is rotated away from the y-axis<BR>
zAngleR, the angle the view is rotated away from the z-axis<BR>
offsetX, Y, and Z, the center of the view<BR>
<BR>
[sd 8/14/98]<BR>


## Examples
```pascal
PROCEDURE Example;

VAR

	xAngleR, yAngelR, zAngleR, offsetX, offsetY, offsetZ :REAL;

BEGIN

	GetView(xAngleR, yAngelR, zAngleR, offsetX, offsetY, offsetZ);

	Message(xAngleR, ' ', yAngelR, ' ', zAngleR, ' ', offsetX, ' ', offsetY, ' ', offsetZ);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks8.0
## Category
* View / Zoom


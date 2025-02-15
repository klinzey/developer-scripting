# Move3DObj

## Description
Procedure Move3DObj moves the referenced object a specified  distance from its current location. Movement distances are calculated from the 3D center of the object. 

```pascal
PROCEDURE Move3DObj(
				h         : HANDLE;
				xDistance : REAL (Coordinate);
				yDistance : REAL (Coordinate);
				zDistance : REAL (Coordinate));
```

```python

def vs.Move3DObj(h, xDistance, yDistance, zDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|xDistance|REAL (Coordinate)|X offset distance.|
|yDistance|REAL (Coordinate)|Y offset distance.|
|zDistance|REAL (Coordinate)|Z offset distance.|

## Examples
```pascal
Move3DObj(HandleToObj,2,4,0);
```

## Version
Availability: from MiniCAD
## Category
* Object Editing


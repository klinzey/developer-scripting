# PickObject

## Description
Function PickObject returns a handle to an object in the document. The function receives a coordinate location, specified by parameter p, and checks this location for the presence of an object. If an object exists at the location, the function returns a handle to the object.&lt;BR&gt;


```pascal
FUNCTION PickObject(p : REAL) : HANDLE;
```

```python

def vs.PickObject(p):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Coordinate location to test for object.|

## Examples
```pascal
FUNCTION UserObjectPick :HANDLE;

VAR 

	x, y :REAL;

BEGIN

	GetPt(x, y);

	UserObjectPick := PickObject(x, y);

END;




```

## See Also
VS Functions:
[GetPickObjectInfo](GetPickObjectInfo.md)| [ForEachObjectAtPoint](ForEachObjectAtPoint.md)

## Version
Availability: from MiniCAD
## Category
* Utility


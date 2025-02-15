# GetFillIAxisEndPoint

## Description
Gets the I-axis end point of the fill.&lt;BR&gt;
&lt;BR&gt;
Note: only works with 2D objects that have a gradient or image fill.

```pascal
PROCEDURE GetFillIAxisEndPoint(
				objectHandle       : HANDLE;
				VAR xIAxisEndPoint : REAL;
				VAR yIAxisEndPoint : REAL);
```

```python

def vs.GetFillIAxisEndPoint(objectHandle):
    return (xIAxisEndPoint, yIAxisEndPoint)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to the object with fill.|
|xIAxisEndPoint|REAL|X coordinate of I-axis point.|
|yIAxisEndPoint|REAL|Y coordinate of I-axis point.|

## Examples
```pascal
GetFillIAxisEndPoint(objectHandle, xIAxis, yIAxis);
```

## Version
Availability: from VectorWorks10.0
## Category
* Object Attributes


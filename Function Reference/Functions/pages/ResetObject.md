# ResetObject

## Description
Update the specified object using the current settings and parameter values.  This will reset the bounding box of the object.  If the object is in a wall, then the wall is reset also.  &lt;BR&gt;
&lt;BR&gt;
An object of any type may be passed to this function to have its boundary reset.  The following object types will be reset in a way that is appropriate for each type: Plug-in Object, Symbol Definition, Wall, Roof Container, Bitmap, Picture, Dimension, Extrude, Multiple Extrude, Sweep, Polygon, Polyline, Worksheet.

```pascal
PROCEDURE ResetObject(objectHandle : HANDLE);
```

```python

def vs.ResetObject(objectHandle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|Handle to the object to be reset.|

## Version
Availability: from VectorWorks10.0
## Category
* Utility


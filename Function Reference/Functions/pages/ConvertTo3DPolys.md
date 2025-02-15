# ConvertTo3DPolys

## Description
Converts an object to 3D polygons. This function successfully converts rectangles, circles, arcs, polylines, polygons, ovals, lines, straight walls, curved walls, and roofs.&lt;BR&gt;


```pascal
FUNCTION ConvertTo3DPolys(original : HANDLE) : HANDLE;
```

```python

def vs.ConvertTo3DPolys(original):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|original|HANDLE|Handle to the original object.|

## Examples
```pascal
PROCEDURE Example;

VAR

	h :HANDLE;

BEGIN

	h := ConvertTo3DPolys(FSActLayer);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks10.0
## Category
* Objects - 3D


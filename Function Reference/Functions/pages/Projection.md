# Projection

## Description
Procedure Projection sets the projection mode of a Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
Parameters viewDistance, clip1, and clip2 are used only in perspective projection mode.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Projection(
				proj         : INTEGER;
				rMode        : INTEGER;
				viewDistance : REAL (Coordinate);
				clip1        : REAL;
				clip2        : REAL);
```

```python

def vs.Projection(proj, rMode, viewDistance, clip1, clip2):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|proj|INTEGER|Projection mode of document.|
|rMode|INTEGER|Render mode of document.|
|viewDistance|REAL (Coordinate)|View length.|
|clip1|REAL|Top left coordinate of clipping rectangle.|
|clip2|REAL|Bottom right coordinate of clipping rectangle.|

## Examples
```pascal
Projection(1,2,3',-2,-2,2,2);


```

## Version
Availability: from MiniCAD4.0
## Category
* View / Zoom


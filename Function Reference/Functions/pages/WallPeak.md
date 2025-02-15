# WallPeak

## Description
Creates a wall peak of the specified height at a specified distance from the wall start point.&lt;BR&gt;
&lt;BR&gt;
There is no error checking of the distance or peak height parameters; it is left to the programmer to ensure that the parameter values are valid.&lt;BR&gt;


```pascal
PROCEDURE WallPeak(
				alongDistance  : REAL (Coordinate);
				heightDistance : REAL (Coordinate));
```

```python

def vs.WallPeak(alongDistance, heightDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|alongDistance|REAL (Coordinate)|Location of peak (measured from wall start point).|
|heightDistance|REAL (Coordinate)|Elevation of wall peak.|

## Examples
```pascal
SetZVal(0',8');

Wall(0,0,7,0);

WallPeak(3'-6&quot;,9'-0&quot;);

{creates a 9' wall peak 3'-6&quot; from the start point of the wall}


```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Walls


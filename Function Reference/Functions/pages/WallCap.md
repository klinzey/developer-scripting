# WallCap

## Description
Procedure WallCap creates a wall cap on a newly created wall object.&lt;BR&gt;
&lt;BR&gt;
Specifying nonzero values for the cap offset values will create angled wall caps.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE WallCap(
				atStart          : BOOLEAN;
				closed           : BOOLEAN;
				round            : BOOLEAN;
				rightOffDistance : REAL (Coordinate);
				leftOffDistance  : REAL (Coordinate));
```

```python

def vs.WallCap(atStart, closed, round, rightOffDistance, leftOffDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|atStart|BOOLEAN|Start-end location of wall cap.|
|closed|BOOLEAN|Controls display status of cap.|
|round|BOOLEAN|Specifies flat or round cap.|
|rightOffDistance|REAL (Coordinate)|Right extension of wall line beyond end point.|
|leftOffDistance|REAL (Coordinate)|Left extension of wall line beyond end point.|

## Examples
```pascal
Wall(0,0,7',0);

WallCap(True, True, False, 1.0', 0.0);

{sets the cap status of the starting cap of the wall as flat cap, bevelled, with the right side extending 1' beyond the wall end point}
```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Walls


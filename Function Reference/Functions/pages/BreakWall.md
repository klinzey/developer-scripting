# BreakWall

## Description
Procedure BreakWall creates a break in a wall object on the left or the right at a specified offset location.&lt;BR&gt;


```pascal
PROCEDURE BreakWall(
				offsetDistance     : REAL (Coordinate);
				breakWidthDistance : REAL (Coordinate);
				right              : BOOLEAN);
```

```python

def vs.BreakWall(offsetDistance, breakWidthDistance, right):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|offsetDistance|REAL (Coordinate)|Offset distance from wall start.|
|breakWidthDistance|REAL (Coordinate)|Width of wall break.|
|right|BOOLEAN|Left-right edge status of break.|

## Examples
```pascal
MoveTo(2,3);

WallTo(7,3);

BreakWall(3&quot;,1&quot;,True);

{creates a right hand 1&quot; wall break 3&quot; from the start of the wall}
```

## Version
Availability: from MiniCAD4.0
## Category
* Objects - Walls


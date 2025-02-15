# SetWallCornerHeights

## Description
Sets the corner heights of a wall or round wall.

```pascal
FUNCTION SetWallCornerHeights(
				theWall           : HANDLE;
				startHeightTop    : REAL (Coordinate);
				startHeightBottom : REAL (Coordinate);
				endHeightTop      : REAL (Coordinate);
				endHeightBottom   : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetWallCornerHeights(theWall, startHeightTop, startHeightBottom, endHeightTop, endHeightBottom):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall or round wall|
|startHeightTop|REAL (Coordinate)|The height of the start top corner|
|startHeightBottom|REAL (Coordinate)|The height of the start bottom corner|
|endHeightTop|REAL (Coordinate)|The height of the end top corner|
|endHeightBottom|REAL (Coordinate)|The height of the end bottom corner|

## Returns
Whether or not the call succeeded

## See Also
VS Functions:
[GetWallCornerHeights](GetWallCornerHeights.md)

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Walls


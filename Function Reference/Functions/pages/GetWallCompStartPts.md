# GetWallCompStartPts

## Description
Gets the start points of a wall component.

```pascal
PROCEDURE GetWallCompStartPts(
				wall            : HANDLE;
				componentIndex  : INTEGER;
				VAR leftPoint   : REAL;
				VAR centerPoint : REAL;
				VAR rightPoint  : REAL);
```

```python

def vs.GetWallCompStartPts(wall, componentIndex):
    return (leftPoint, centerPoint, rightPoint)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wall|HANDLE|The wall or round wall|
|componentIndex|INTEGER|The component index|
|leftPoint|REAL|Returns the left start point of the component|
|centerPoint|REAL|Returns the center start point of the component|
|rightPoint|REAL|Returns the right start point of the component|

## Returns
None

## See Also
VS Functions:
[GetWallCompEndPts](GetWallCompEndPts.md)

## Version
Availability: from Vectorworks 2015
## Category
* Objects - Walls


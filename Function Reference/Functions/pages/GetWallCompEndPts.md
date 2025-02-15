# GetWallCompEndPts

## Description
Gets the end points of a wall component.

```pascal
PROCEDURE GetWallCompEndPts(
				wall            : HANDLE;
				componentIndex  : INTEGER;
				VAR leftPoint   : REAL;
				VAR centerPoint : REAL;
				VAR rightPoint  : REAL);
```

```python

def vs.GetWallCompEndPts(wall, componentIndex):
    return (leftPoint, centerPoint, rightPoint)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wall|HANDLE|The wall or round wall|
|componentIndex|INTEGER|The component index|
|leftPoint|REAL|Returns the left end point of the component|
|centerPoint|REAL|Returns the center end point of the component|
|rightPoint|REAL|Returns the right end point of the component|

## Returns
None

## See Also
VS Functions:
[GetWallCompStartPts](GetWallCompStartPts.md)

## Version
Availability: from Vectorworks 2015
## Category
* Objects - Walls


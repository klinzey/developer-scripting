# AddSymToWall

## Description
Procedure AddSymToWall inserts a specified symbol into the referenced wall.

```pascal
PROCEDURE AddSymToWall(
				wallHd         : HANDLE;
				offDistance    : REAL (Coordinate);
				heightDistance : REAL (Coordinate);
				flip           : BOOLEAN;
				right          : BOOLEAN;
				symbolName     : STRING);
```

```python

def vs.AddSymToWall(wallHd, offDistance, heightDistance, flip, right, symbolName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallHd|HANDLE|Handle to wall.|
|offDistance|REAL (Coordinate)|Offset distance from wall start.|
|heightDistance|REAL (Coordinate)|Elevation of symbol.|
|flip|BOOLEAN|Flipped status of symbol.|
|right|BOOLEAN|Left-right orientation of symbol.|
|symbolName|STRING|Name of symbol to insert in wall.|

## Remarks
See AddSymToWallEdge<BR>
[sd 8/13/98]

## Examples
```pascal
AddSymToWall(HandleToWall,3',0',FALSE,FALSE,'Door-1');
```

## See Also
VS Functions:
[AddSymToWallEdge](AddSymToWallEdge.md)

## Version
Availability: from MiniCAD6.0
## Category
* Objects - Walls


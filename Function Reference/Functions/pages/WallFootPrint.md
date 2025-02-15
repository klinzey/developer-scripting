# WallFootPrint

## Description
Returns the handle of a polyline representing the footprint of a wall.

```pascal
FUNCTION WallFootPrint(wallHandle : HANDLE) : HANDLE;
```

```python

def vs.WallFootPrint(wallHandle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallHandle|HANDLE|Handle to the wall|

## Returns
Returns the handle of a polyline representing the footprint of a wall.

## Examples
```pascal
PROCEDURE GetWallFootPrint;

VAR

	h1, h2 :HANDLE;

BEGIN

	h1 := FSActLayer;

	h2 := WallFootPrint(h1);

END;

RUN(GetWallFootPrint);


```

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Walls


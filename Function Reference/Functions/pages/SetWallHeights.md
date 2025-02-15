# SetWallHeights

## Description
Sets the wall heights of an unstyled wall. Will return false for a styled wall.

```pascal
FUNCTION SetWallHeights(
				h               : HANDLE;
				startHtDistance : REAL (Coordinate);
				endHtDistance   : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetWallHeights(h, startHtDistance, endHtDistance):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|startHtDistance|REAL (Coordinate)||
|endHtDistance|REAL (Coordinate)||

## Examples
```pascal
PROCEDURE Example;

VAR

	h :HANDLE;

	boo :BOOLEAN;

BEGIN

	CallTool(-208);

	h := FSActLayer;

	boo := SetWallHeights(h, 12, 23);

END;

RUN(Example);


```

## Version
```diff
- SetWallHeights is obsolete as of Vectorworks 2012
```

Availability: from VectorWorks12.0
## Category
* Objects - Walls


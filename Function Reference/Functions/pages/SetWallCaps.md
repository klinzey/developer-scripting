# SetWallCaps

## Description
Set the wall's caps.

```pascal
FUNCTION SetWallCaps(
				theWall  : HANDLE;
				leftCap  : BOOLEAN;
				rightCap : BOOLEAN;
				round    : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetWallCaps(theWall, leftCap, rightCap, round):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theWall|HANDLE|The wall.|
|leftCap|BOOLEAN|Whether or not the wall has a left cap.|
|rightCap|BOOLEAN|Whether or not the wall has a right cap.|
|round|BOOLEAN|Whether or not the wall's caps are round.|

## Returns
Returns success status.

## See Also
VS Functions:
[GetWallCaps](GetWallCaps.md)

## Version
Availability: from VectorWorks12.5
## Category
* Objects - Walls


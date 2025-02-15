# WallHeight

## Description
Procedure WallHeight returns the wall heights of the referenced wall object.&lt;BR&gt;


```pascal
PROCEDURE WallHeight(
				wallHd      : HANDLE;
				VAR startHt : REAL;
				VAR endHt   : REAL);
```

```python

def vs.WallHeight(wallHd):
    return (startHt, endHt)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallHd|HANDLE|Handle to wall.|
|startHt|REAL|Returns start height of wall.|
|endHt|REAL|Returns end height of wall.|

## Version
```diff
- WallHeight is obsolete as of Vectorworks 2012
```

Availability: from MiniCAD6.0
## Category
* Objects - Walls


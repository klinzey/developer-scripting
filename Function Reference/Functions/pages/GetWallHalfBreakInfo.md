# GetWallHalfBreakInfo

## Description
Gets the start point, center point and end point of a half break in a wall along the wall line.

```pascal
FUNCTION GetWallHalfBreakInfo(
				wallH        : HANDLE;
				breakIndex   : INTEGER;
				VAR startPt  : REAL;
				VAR centerPt : REAL;
				VAR endPt    : REAL) : BOOLEAN;
```

```python

def vs.GetWallHalfBreakInfo(wallH, breakIndex):
    return (BOOLEAN, startPt, centerPt, endPt)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallH|HANDLE||
|breakIndex|INTEGER||
|startPt|REAL||
|centerPt|REAL||
|endPt|REAL||

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Walls


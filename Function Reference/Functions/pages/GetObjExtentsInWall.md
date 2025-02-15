# GetObjExtentsInWall

## Description
Gets the extents of a Plugin object or symbol that is in a wall.  Returns the object's start point and end point along the wall line.

```pascal
FUNCTION GetObjExtentsInWall(
				symH        : HANDLE;
				wallH       : HANDLE;
				VAR startPt : REAL;
				VAR endPt   : REAL) : BOOLEAN;
```

```python

def vs.GetObjExtentsInWall(symH, wallH):
    return (BOOLEAN, startPt, endPt)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|symH|HANDLE||
|wallH|HANDLE||
|startPt|REAL||
|endPt|REAL||

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Walls


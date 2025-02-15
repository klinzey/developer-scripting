# DTM6_GetZatXY

## Description
Get the elevation at specified x,y on the specified DTM. Returns false if the DTM doesnt exist or the point is outside the DTM. TINType - 0:Existing; 1:Proposed; 2:Current

```pascal
FUNCTION DTM6_GetZatXY(
				hDTMObject : HANDLE;
				TINType    : INTEGER;
				x          : REAL;
				y          : REAL;
				VAR outZ   : REAL) : BOOLEAN;
```

```python

def vs.DTM6_GetZatXY(hDTMObject, TINType, x, y):
    return (BOOLEAN, outZ)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hDTMObject|HANDLE||
|TINType|INTEGER||
|x|REAL||
|y|REAL||
|outZ|REAL||

## Version
Availability: from Vectorworks 2011
## Category
* SiteModel Interface Library


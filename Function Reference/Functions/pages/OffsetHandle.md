# OffsetHandle

## Description
Creates a group of lines which represent the weighted medial axis of given polygon.

```pascal
FUNCTION OffsetHandle(
				h                : HANDLE;
				offsetDistance   : REAL;
				EdgeRestoration  : BOOLEAN;
				FilletSharpEdges : BOOLEAN) : HANDLE;
```

```python

def vs.OffsetHandle(h, offsetDistance, EdgeRestoration, FilletSharpEdges):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|offsetDistance|REAL||
|EdgeRestoration|BOOLEAN||
|FilletSharpEdges|BOOLEAN||

## Version
Availability: from Vectorworks 2014
## Category
* Object Editing


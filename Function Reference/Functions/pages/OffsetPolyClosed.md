# OffsetPolyClosed

## Description
Offsets a polyline or polygon, then uses the original geometry to construct a closed profile.  

```pascal
FUNCTION OffsetPolyClosed(
				obj           : HANDLE;
				offset        : REAL;
				smoothCorners : BOOLEAN) : HANDLE;
```

```python

def vs.OffsetPolyClosed(obj, offset, smoothCorners):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE||
|offset|REAL||
|smoothCorners|BOOLEAN||

## Version
Availability: from Vectorworks 2018
## Category
* Objects - 2D


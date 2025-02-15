# GetObjStoryBoundsAt

## Description
Return the story bound ID of the specified story bound index. The index is between 1 and the result of GetObjStoryBoundsCnt.

```pascal
FUNCTION GetObjStoryBoundsAt(
				object : HANDLE;
				index  : INTEGER) : INTEGER;
```

```python

def vs.GetObjStoryBoundsAt(object, index):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object.|
|index|INTEGER|Index of the story bound which ID will be returned. This index should be between 1 and the result of GetObjStoryBoundsCnt.|

## Returns
Return the story bound ID.

## See Also
VS Functions:
[HasObjStoryBounds](HasObjStoryBounds.md)| [HasObjStoryBound](HasObjStoryBound.md)| [GetObjStoryBound](GetObjStoryBound.md)| [SetObjectStoryBound](SetObjectStoryBound.md)| [DelObjStoryBounds](DelObjStoryBounds.md)| [DelObjStoryBound](DelObjStoryBound.md)| [GetObjStoryBoundsCnt](GetObjStoryBoundsCnt.md)| [GetObjStoryBoundsAt](GetObjStoryBoundsAt.md)

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Architectural


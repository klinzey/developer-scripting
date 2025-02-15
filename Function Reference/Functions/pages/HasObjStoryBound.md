# HasObjStoryBound

## Description
Determine if the object has the specified story bound ID present.

```pascal
FUNCTION HasObjStoryBound(
				object  : HANDLE;
				boundID : INTEGER) : BOOLEAN;
```

```python

def vs.HasObjStoryBound(object, boundID):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object.|
|boundID|INTEGER|The identifier of the story bound.|

## Returns
Retrun TRUE if the story bound ID is present. Otherwise - FALSE.

## See Also
VS Functions:
[HasObjStoryBounds](HasObjStoryBounds.md)| [HasObjStoryBound](HasObjStoryBound.md)| [GetObjStoryBound](GetObjStoryBound.md)| [SetObjectStoryBound](SetObjectStoryBound.md)| [DelObjStoryBounds](DelObjStoryBounds.md)| [DelObjStoryBound](DelObjStoryBound.md)| [GetObjStoryBoundsCnt](GetObjStoryBoundsCnt.md)| [GetObjStoryBoundsAt](GetObjStoryBoundsAt.md)

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Architectural


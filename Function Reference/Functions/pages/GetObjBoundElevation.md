# GetObjBoundElevation

## Description
Get the elevation of the specified bound ID relative to the object's layer.

```pascal
FUNCTION GetObjBoundElevation(
				object  : HANDLE;
				boundID : INTEGER) : REAL;
```

```python

def vs.GetObjBoundElevation(object, boundID):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object.|
|boundID|INTEGER|The identifier of the story bound.|

## Returns
Return the elevation of the specified bound ID relative to the object's layer.

## See Also
VS Functions:
[HasObjStoryBounds](HasObjStoryBounds.md)| [HasObjStoryBound](HasObjStoryBound.md)| [GetObjStoryBound](GetObjStoryBound.md)| [SetObjectStoryBound](SetObjectStoryBound.md)| [DelObjStoryBounds](DelObjStoryBounds.md)| [DelObjStoryBound](DelObjStoryBound.md)| [GetObjStoryBoundsCnt](GetObjStoryBoundsCnt.md)| [GetObjStoryBoundsAt](GetObjStoryBoundsAt.md)

## Version
Availability: from Vectorworks 2012
## Category
* Objects - Architectural


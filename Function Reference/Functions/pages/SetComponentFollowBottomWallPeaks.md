# SetComponentFollowBottomWallPeaks

## Description
Sets the follow bottom wall peaks flag of a component in an object.

```pascal
FUNCTION SetComponentFollowBottomWallPeaks(
				object                : HANDLE;
				componentIndex        : INTEGER;
				followBottomWallPeaks : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetComponentFollowBottomWallPeaks(object, componentIndex, followBottomWallPeaks):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|
|componentIndex|INTEGER|The index of the component.|
|followBottomWallPeaks|BOOLEAN|Whether or not the component will follow bottom wall peaks.|

## See Also
VS Functions:
[GetComponentFollowBottomWallPeaks](GetComponentFollowBottomWallPeaks.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


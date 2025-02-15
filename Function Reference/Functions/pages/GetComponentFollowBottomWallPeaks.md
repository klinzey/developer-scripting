# GetComponentFollowBottomWallPeaks

## Description
Gets the follow bottom wall peaks flag of a component in an object.

```pascal
FUNCTION GetComponentFollowBottomWallPeaks(
				object                    : HANDLE;
				componentIndex            : INTEGER;
				VAR followBottomWallPeaks : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetComponentFollowBottomWallPeaks(object, componentIndex):
    return (BOOLEAN, followBottomWallPeaks)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|
|componentIndex|INTEGER|The index of the component.|
|followBottomWallPeaks|BOOLEAN|Returns whether or not the component is following bottom wall peaks.|

## See Also
VS Functions:
[SetComponentFollowBottomWallPeaks](SetComponentFollowBottomWallPeaks.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


# GetComponentFollowTopWallPeaks

## Description
Gets the follow top wall peaks flag of a component in an object.

```pascal
FUNCTION GetComponentFollowTopWallPeaks(
				object                 : HANDLE;
				componentIndex         : INTEGER;
				VAR followTopWallPeaks : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetComponentFollowTopWallPeaks(object, componentIndex):
    return (BOOLEAN, followTopWallPeaks)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|
|componentIndex|INTEGER|The index of the component.|
|followTopWallPeaks|BOOLEAN|Returns whether or not the component is following top wall peaks.|

## See Also
VS Functions:
[SetComponentFollowTopWallPeaks](SetComponentFollowTopWallPeaks.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Architectural


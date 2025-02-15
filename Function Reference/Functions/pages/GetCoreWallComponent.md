# GetCoreWallComponent

## Description
Gets the core wall component of an object.

```pascal
FUNCTION GetCoreWallComponent(object : HANDLE) : INTEGER;
```

```python

def vs.GetCoreWallComponent(object):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, Wall Style, or the Wall Preferences.|

## Returns
The index of the core wall component.  If it is 0, there is no core wall component.

## See Also
VS Functions:
[SetCoreWallComponent](SetCoreWallComponent.md)

## Version
Availability: from Vectorworks 2010
## Category
* Objects - Architectural


# GetCompInsertLoc

## Description
Gets the component insert location of the object.

```pascal
FUNCTION GetCompInsertLoc(object : HANDLE) : INTEGER;
```

```python

def vs.GetCompInsertLoc(object):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, Wall Style, or the Wall Preferences.|

## Returns
The component insert location of the object.<BR>
<BR>
0 - None<BR>
1 - Left<BR>
2 - Center<BR>
3 - Right

## See Also
VS Functions:
[SetCompInsertLoc](SetCompInsertLoc.md)

## Version
Availability: from Vectorworks 2023
## Category
* Objects - Architectural


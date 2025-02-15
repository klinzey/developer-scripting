# GetVPLrOvrdCount

## Description
Retrieves the number of layer overrides.

```pascal
FUNCTION GetVPLrOvrdCount(viewportHandle : HANDLE) : INTEGER;
```

```python

def vs.GetVPLrOvrdCount(viewportHandle):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE|The viewport handle.|

## Returns
Returns the number of layer overrides associated with the specified viewport.<BR>
If the handle is invalid, returns -1.

## See Also
VS Functions:
[GetVPLrOvrdHandle](GetVPLrOvrdHandle.md)

## Version
Availability: from Vectorworks 2014
## Category
* Viewports


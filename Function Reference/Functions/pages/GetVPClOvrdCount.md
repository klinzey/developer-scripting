# GetVPClOvrdCount

## Description
Returns the number of class overrides associated with a particular viewport.

```pascal
FUNCTION GetVPClOvrdCount(viewportHandle : HANDLE) : INTEGER;
```

```python

def vs.GetVPClOvrdCount(viewportHandle):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE|The viewport handle.|

## Returns
Returns the number of class overrides associated with the given viewport.<BR>
If the handle is invalid, returns -1.

## See Also
VS Functions:
[GetVPClOvrdName](GetVPClOvrdName.md)

## Version
Availability: from Vectorworks 2014
## Category
* Viewports


# GetVPLrOvrdHandle

## Description
Retrieves the handle of the layer overridden at the specified index in the overrides list.

```pascal
FUNCTION GetVPLrOvrdHandle(
				viewportHandle : HANDLE;
				index          : INTEGER) : HANDLE;
```

```python

def vs.GetVPLrOvrdHandle(viewportHandle, index):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE|The viewport handle.|
|index|INTEGER|The index into the layer overrides list.|

## Returns
Returns a handle to the layer overriden at the given index.<BR>
Returns 0 if the index is out of range.

## See Also
VS Functions:
[GetVPLrOvrdCount](GetVPLrOvrdCount.md)

## Version
Availability: from Vectorworks 2014
## Category
* Viewports


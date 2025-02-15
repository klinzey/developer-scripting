# GetFillSpace

## Description
Returns the handle of the index-th fill space in the specified object's aux list.

```pascal
FUNCTION GetFillSpace(
				h     : HANDLE;
				index : INTEGER) : HANDLE;
```

```python

def vs.GetFillSpace(h, index):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to the object containing the fill space.|
|index|INTEGER|Index of the fill space to be returned.|

## Returns
Handle to the index-th fill space in h's aux list.

## Version
Availability: from Vectorworks 2018
## Category
* Object Attributes


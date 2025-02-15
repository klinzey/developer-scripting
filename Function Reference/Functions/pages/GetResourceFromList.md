# GetResourceFromList

## Description
Returns the indicated resource from the indicated resource list, if the resource is in the current document.  Otherwise it returns nil.

```pascal
FUNCTION GetResourceFromList(
				listID : LONGINT;
				index  : LONGINT) : HANDLE;
```

```python

def vs.GetResourceFromList(listID, index):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|listID|LONGINT|an ID for a resource list created by the BuildResourceList command.|
|index|LONGINT|an index into the list.|

## Examples
```pascal
hatch := GetResourceFromList(listID, index);

if (hatch = NIL) then

	hatch := ImportResourceToCurrentFile(listID, index);


```

## Version
Availability: from VectorWorks12.0
## Category
* Document List Handling


# ImportResourceToCurrentFile

## Description
Imports the indicated resource from the specified list to the current file, if it is not already in the current file, and returns the handle to the resource.

```pascal
FUNCTION ImportResourceToCurrentFile(
				listID : LONGINT;
				index  : LONGINT) : HANDLE;
```

```python

def vs.ImportResourceToCurrentFile(listID, index):
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


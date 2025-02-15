# BuildResourceListN

## Description
Build a resource list from the specified file.

```pascal
FUNCTION BuildResourceListN(
				type         : INTEGER;
				fullPath     : DYNARRAY[] of CHAR;
				VAR numItems : LONGINT) : LONGINT;
```

```python

def vs.BuildResourceListN(type, fullPath):
    return (LONGINT, numItems)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|type|INTEGER|the type of resource to put in the list|
|fullPath|DYNARRAY[] of CHAR|The path to the file that provides the resources.|
|numItems|LONGINT|the number of items in the list built|

## See Also
VS Functions:
[BuildResourceList](BuildResourceList.md)

## Version
Availability: from Vectorworks 2013
## Category
* Document List Handling


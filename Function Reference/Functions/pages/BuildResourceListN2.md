# BuildResourceListN2

## Description
Build a resource list from the specified file.

```pascal
FUNCTION BuildResourceListN2(
				type              : INTEGER;
				fullPath          : DYNARRAY[] of CHAR;
				VAR numItems      : LONGINT;
				useDefaultContent : BOOLEAN) : LONGINT;
```

```python

def vs.BuildResourceListN2(type, fullPath, useDefaultContent):
    return (LONGINT, numItems)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|type|INTEGER|the type of resource to put in the list|
|fullPath|DYNARRAY[] of CHAR|The path to the file that provides the resources.|
|numItems|LONGINT|the number of items in the list built|
|useDefaultContent|BOOLEAN|determine if the list should contain default content|

## See Also
VS Functions:
[BuildResourceListN](BuildResourceListN.md)| [BuildResourceList](BuildResourceList.md)| [BuildResourceList2](BuildResourceList2.md)

## Version
Availability: from Vectorworks 2014
## Category
* Document List Handling


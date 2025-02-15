# ws2GetMenuAt

## Description
Workspace advanced APIs. Return the universal name of the specified index inside the provided menu path See 'ws2GetMenusCnt'.

```pascal
FUNCTION ws2GetMenuAt(
				menuPath : DYNARRAY[] of CHAR;
				index    : INTEGER) : DYNARRAY[] of CHAR;
```

```python

def vs.ws2GetMenuAt(menuPath, index):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|menuPath|DYNARRAY[] of CHAR||
|index|INTEGER||

## Version
Availability: from Vectorworks 2021
## Category
* Workspaces


# GetNumberOfComponents

## Description
Gets the number of components in an object.

```pascal
FUNCTION GetNumberOfComponents(
				object            : HANDLE;
				VAR numComponents : INTEGER) : BOOLEAN;
```

```python

def vs.GetNumberOfComponents(object):
    return (BOOLEAN, numComponents)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|numComponents|INTEGER|Returns the number of components.|

## Version
Availability: from VectorWorks12.0
## Category
* Objects - Architectural


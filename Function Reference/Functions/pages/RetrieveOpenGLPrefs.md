# RetrieveOpenGLPrefs

## Description
Retrieves the current OpenGL rendering preferences from data stored in the current drawing.

```pascal
PROCEDURE RetrieveOpenGLPrefs(
				VAR useTextures        : BOOLEAN;
				VAR tessellationDetail : INTEGER;
				VAR useNURBS           : BOOLEAN);
```

```python

def vs.RetrieveOpenGLPrefs():
    return (useTextures, tessellationDetail, useNURBS)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|useTextures|BOOLEAN||
|tessellationDetail|INTEGER||
|useNURBS|BOOLEAN||

## Version
Availability: from Vectorworks 2014
## Category
* View / Zoom


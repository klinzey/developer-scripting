# SetOpenGLPrefs

## Description
Sets the current OpenGL rendering preferences from data passed in.

```pascal
PROCEDURE SetOpenGLPrefs(
				VAR useTextures        : BOOLEAN;
				VAR tessellationDetail : INTEGER;
				VAR useNURBS           : BOOLEAN);
```

```python

def vs.SetOpenGLPrefs():
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
* Textures


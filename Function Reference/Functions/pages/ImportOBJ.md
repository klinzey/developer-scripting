# ImportOBJ

## Description
Imports Wavefront (*.obj) files.

```pascal
FUNCTION ImportOBJ(
				fileName    : DYNARRAY[] of CHAR;
				bAllMatAsRW : BOOLEAN) : BOOLEAN;
```

```python

def vs.ImportOBJ(fileName, bAllMatAsRW):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Full file path.|
|bAllMatAsRW|BOOLEAN|Imports all materials as Renderworks textures.|

## Returns
TRUE if import is successful.

## Version
Availability: from Vectorworks 2016
## Category
* ImportExport


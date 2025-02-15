# ImportSketchUp

## Description
Imports SketchUp ( *.skp)  files.

```pascal
FUNCTION ImportSketchUp(
				filePath      : DYNARRAY[] of CHAR;
				bImportAsMesh : BOOLEAN) : BOOLEAN;
```

```python

def vs.ImportSketchUp(filePath, bImportAsMesh):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filePath|DYNARRAY[] of CHAR|Full file path.|
|bImportAsMesh|BOOLEAN|Import as a Mesh or as 3D polys. Mesh = TRUE.|

## Returns
TRUE if import is successful.

## Version
Availability: from Vectorworks 2016
## Category
* ImportExport


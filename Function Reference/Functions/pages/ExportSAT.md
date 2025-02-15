# ExportSAT

## Description
Export the selection into a SAT file.

```pascal
FUNCTION ExportSAT(
				filePath       : DYNARRAY[] of CHAR;
				solidAsSurface : BOOLEAN) : BOOLEAN;
```

```python

def vs.ExportSAT(filePath, solidAsSurface):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filePath|DYNARRAY[] of CHAR|Output file path.|
|solidAsSurface|BOOLEAN||

## Returns
Return TRUE if successful.

## Version
Availability: from Vectorworks 2013
## Category
* File I/O


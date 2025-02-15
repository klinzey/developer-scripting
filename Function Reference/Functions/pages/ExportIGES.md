# ExportIGES

## Description
Export the document in 3D IGES file.

```pascal
FUNCTION ExportIGES(
				fileName             : DYNARRAY[] of CHAR;
				exportSolidAsSurface : BOOLEAN) : BOOLEAN;
```

```python

def vs.ExportIGES(fileName, exportSolidAsSurface):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Output file path.|
|exportSolidAsSurface|BOOLEAN|Export solit objects as surface.|

## Returns
Return TRUE if succeeded.

## See Also
VS Functions:
[ImportIGES](ImportIGES.md)

## Version
Availability: from Vectorworks 2014
## Category
* File I/O


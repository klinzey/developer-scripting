# ImportSAT

## Description
Import a SAT file.

```pascal
FUNCTION ImportSAT(
				filePath    : DYNARRAY[] of CHAR;
				doSingleSym : BOOLEAN) : HANDLE;
```

```python

def vs.ImportSAT(filePath, doSingleSym):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|filePath|DYNARRAY[] of CHAR|full path to the file for import|
|doSingleSym|BOOLEAN|import the file as a symbol|

## Returns
Return handle to the imported symbol, or to the first imported object (first selected).

## Version
Availability: from Vectorworks 2013
## Category
* File I/O


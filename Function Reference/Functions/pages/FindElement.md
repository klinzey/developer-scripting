# FindElement

## Description
Finds the specified element by name.

```pascal
FUNCTION FindElement(
				XMLHandle        : LONGINT;
				startElementPath : DYNARRAY[] of CHAR;
				searchElement    : DYNARRAY[] of CHAR;
				VAR foundPath    : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.FindElement(XMLHandle, startElementPath, searchElement):
    return (INTEGER, foundPath)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|startElementPath|DYNARRAY[] of CHAR||
|searchElement|DYNARRAY[] of CHAR||
|foundPath|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


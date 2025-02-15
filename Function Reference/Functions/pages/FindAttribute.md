# FindAttribute

## Description
Finds the specified attribute by name.

```pascal
FUNCTION FindAttribute(
				XMLHandle          : LONGINT;
				startElementPath   : DYNARRAY[] of CHAR;
				searchAttribute    : DYNARRAY[] of CHAR;
				VAR foundPath      : DYNARRAY[] of CHAR;
				VAR attributeValue : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.FindAttribute(XMLHandle, startElementPath, searchAttribute):
    return (INTEGER, foundPath, attributeValue)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|startElementPath|DYNARRAY[] of CHAR||
|searchAttribute|DYNARRAY[] of CHAR||
|foundPath|DYNARRAY[] of CHAR||
|attributeValue|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


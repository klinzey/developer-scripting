# GetNextElement

## Description
Returns the next element (sibling) of the given element.

```pascal
FUNCTION GetNextElement(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				VAR value   : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.GetNextElement(XMLHandle, elementPath):
    return (INTEGER, value)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|elementPath|DYNARRAY[] of CHAR||
|value|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


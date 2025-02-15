# GetFirstChild

## Description
Returns first child of given element.

```pascal
FUNCTION GetFirstChild(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				VAR value   : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.GetFirstChild(XMLHandle, elementPath):
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


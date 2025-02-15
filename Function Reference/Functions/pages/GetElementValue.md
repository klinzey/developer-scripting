# GetElementValue

## Description
Gets a value of an element, given a path.

```pascal
FUNCTION GetElementValue(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				VAR value   : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.GetElementValue(XMLHandle, elementPath):
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


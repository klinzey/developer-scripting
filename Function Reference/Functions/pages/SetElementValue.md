# SetElementValue

## Description
Sets a value of an element, given a path.

```pascal
FUNCTION SetElementValue(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				value       : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.SetElementValue(XMLHandle, elementPath, value):
    return INTEGER
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


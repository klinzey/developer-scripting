# GetCDATA

## Description
Gets CDATA section.

```pascal
FUNCTION GetCDATA(
				XMLHandle     : LONGINT;
				elementPath   : DYNARRAY[] of CHAR;
				VAR returnVal : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.GetCDATA(XMLHandle, elementPath):
    return (INTEGER, returnVal)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|elementPath|DYNARRAY[] of CHAR||
|returnVal|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


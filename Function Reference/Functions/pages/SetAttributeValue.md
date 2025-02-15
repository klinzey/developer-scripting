# SetAttributeValue

## Description
Sets a value of an attribute.

```pascal
FUNCTION SetAttributeValue(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				attribute   : DYNARRAY[] of CHAR;
				value       : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.SetAttributeValue(XMLHandle, elementPath, attribute, value):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|elementPath|DYNARRAY[] of CHAR||
|attribute|DYNARRAY[] of CHAR||
|value|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


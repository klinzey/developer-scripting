# GetAttributeValue

## Description
Gets a value of an attribute.

```pascal
FUNCTION GetAttributeValue(
				XMLHandle   : LONGINT;
				elementPath : DYNARRAY[] of CHAR;
				attribute   : DYNARRAY[] of CHAR;
				VAR value   : STRING) : INTEGER;
```

```python

def vs.GetAttributeValue(XMLHandle, elementPath, attribute):
    return (INTEGER, value)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|elementPath|DYNARRAY[] of CHAR||
|attribute|DYNARRAY[] of CHAR||
|value|STRING||

## Version
Availability: from Vectorworks 2011
## Category
* XML


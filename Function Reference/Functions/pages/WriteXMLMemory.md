# WriteXMLMemory

## Description
Creates XML data from an internal DOM tree.

```pascal
FUNCTION WriteXMLMemory(
				XMLHandle   : LONGINT;
				VAR XMLData : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.WriteXMLMemory(XMLHandle):
    return (INTEGER, XMLData)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|XMLData|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML


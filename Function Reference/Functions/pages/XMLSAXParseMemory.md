# XMLSAXParseMemory

## Description
Parse an XML from memory using SAX. 

```pascal
FUNCTION XMLSAXParseMemory(
				XMLHandle    : LONGINT;
				XMLData      : DYNARRAY[] of CHAR;
				nodeCallback : PROCEDURE) : INTEGER;
```

```python

def vs.XMLSAXParseMemory(XMLHandle, XMLData, nodeCallback):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|XMLData|DYNARRAY[] of CHAR||
|nodeCallback|PROCEDURE||

## Version
Availability: from Vectorworks 2011
## Category
* XML SAX


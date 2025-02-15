# XMLSAXEndDocMemory

## Description
Write XML using SAX, end of a document. XMLSAXBeginDocMemory begins a document.

```pascal
FUNCTION XMLSAXEndDocMemory(
				XMLHandle   : LONGINT;
				VAR XMLData : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.XMLSAXEndDocMemory(XMLHandle):
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
* XML SAX


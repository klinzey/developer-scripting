# XMLSAXParseFile

## Description
Parse an XML file using SAX.

```pascal
FUNCTION XMLSAXParseFile(
				XMLHandle    : LONGINT;
				whichPath    : INTEGER;
				filename     : DYNARRAY[] of CHAR;
				nodeCallback : PROCEDURE) : INTEGER;
```

```python

def vs.XMLSAXParseFile(XMLHandle, whichPath, filename, nodeCallback):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|whichPath|INTEGER||
|filename|DYNARRAY[] of CHAR||
|nodeCallback|PROCEDURE||

## Version
Availability: from Vectorworks 2011
## Category
* XML SAX


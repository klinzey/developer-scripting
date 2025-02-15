# XMLSAXBeginDocFile

## Description
Write XML using SAX, begin of a document file. XMLSAXEndDoc ends a document.

```pascal
FUNCTION XMLSAXBeginDocFile(
				XMLHandle : LONGINT;
				whichPath : INTEGER;
				filename  : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.XMLSAXBeginDocFile(XMLHandle, whichPath, filename):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|whichPath|INTEGER||
|filename|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML SAX


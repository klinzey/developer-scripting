# XMLSAXBeginNode

## Description
Write XML using SAX, begin of a node. XMLSAXEndNode ends a node

```pascal
FUNCTION XMLSAXBeginNode(
				XMLHandle : LONGINT;
				nodeName  : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.XMLSAXBeginNode(XMLHandle, nodeName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|nodeName|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML SAX


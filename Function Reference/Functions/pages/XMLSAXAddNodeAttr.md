# XMLSAXAddNodeAttr

## Description
Write XML using SAX, adds a node attributes to a node begun with XMLSAXBeginNode.

```pascal
FUNCTION XMLSAXAddNodeAttr(
				XMLHandle     : LONGINT;
				nodeAttrName  : DYNARRAY[] of CHAR;
				nodeAttrValue : DYNARRAY[] of CHAR) : INTEGER;
```

```python

def vs.XMLSAXAddNodeAttr(XMLHandle, nodeAttrName, nodeAttrValue):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|XMLHandle|LONGINT||
|nodeAttrName|DYNARRAY[] of CHAR||
|nodeAttrValue|DYNARRAY[] of CHAR||

## Version
Availability: from Vectorworks 2011
## Category
* XML SAX


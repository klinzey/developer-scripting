# GetTexMapIntN

## Description
Get map info for specific part of object. partID is texture part, overall is 3. Selector should be1, to return the texture map type integer.

```pascal
FUNCTION GetTexMapIntN(
				obj        : HANDLE;
				texPartID  : LONGINT;
				texLayerID : LONGINT;
				selector   : INTEGER) : INTEGER;
```

```python

def vs.GetTexMapIntN(obj, texPartID, texLayerID, selector):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE||
|texPartID|LONGINT||
|texLayerID|LONGINT|0 for base, &gt;0 for decals|
|selector|INTEGER||

## Version
Availability: from Vectorworks 2010
## Category
* Textures


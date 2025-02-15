# GetTexMapBoolN

## Description
Get map info for specific part of object. partID is texture part, overall is 3. Selector: init:1, flip:2, repH:3, repV:4, long edge:5, worldZ:6, auto align:7

```pascal
FUNCTION GetTexMapBoolN(
				obj        : HANDLE;
				texPartID  : LONGINT;
				texLayerID : LONGINT;
				selector   : INTEGER) : BOOLEAN;
```

```python

def vs.GetTexMapBoolN(obj, texPartID, texLayerID, selector):
    return BOOLEAN
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


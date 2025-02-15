# GetTexMapBool

## Description
Get map info for specific part of object. partID is texture part, overall is 3. Selector: init:1, flip:2, repH:3, repV:4, long edge:5, worldZ:6, auto align:7

```pascal
FUNCTION GetTexMapBool(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER) : BOOLEAN;
```

```python

def vs.GetTexMapBool(h, partID, selector):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||

## Version
```diff
- GetTexMapBool is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


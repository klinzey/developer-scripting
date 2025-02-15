# SetTexMapBool

## Description
Set map info for specific part of object. partID is texture part, overall is 3. Selector: init:1, flip:2, repH:3, repV:4, long edge:5, worldZ:6, auto align:7

```pascal
PROCEDURE SetTexMapBool(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER;
				value    : BOOLEAN);
```

```python

def vs.SetTexMapBool(h, partID, selector, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||
|value|BOOLEAN||

## Version
```diff
- SetTexMapBool is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


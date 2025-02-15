# SetTexMapInt

## Description
Set map info for specific part of object. partID is texture part, overall is 3. Selector should be 1 to set the map type integer.

```pascal
PROCEDURE SetTexMapInt(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER;
				value    : INTEGER);
```

```python

def vs.SetTexMapInt(h, partID, selector, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||
|value|INTEGER||

## Version
```diff
- SetTexMapInt is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


# GetTexMapInt

## Description
Get map info for specific part of object. partID is texture part, overall is 3. Selector should be1, to return the texture map type integer.

```pascal
FUNCTION GetTexMapInt(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER) : INTEGER;
```

```python

def vs.GetTexMapInt(h, partID, selector):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||

## Version
```diff
- GetTexMapInt is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


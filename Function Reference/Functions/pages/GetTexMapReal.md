# GetTexMapReal

## Description
Get map info for specific part of object. partID is texture part, overall is 3. Selector: offsetX:1, offsetY:2, scale2D:3, rotate2D:4, radius:5, matrix mat00 through mat32: 6-17

```pascal
FUNCTION GetTexMapReal(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER) : REAL;
```

```python

def vs.GetTexMapReal(h, partID, selector):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||

## Version
```diff
- GetTexMapReal is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


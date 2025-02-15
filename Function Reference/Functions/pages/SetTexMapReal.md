# SetTexMapReal

## Description
Set map info for specific part of object. partID is texture part, overall is 3. Selector: offsetX:1, offsetY:2, scale2D:3, rotate2D:4, radius:5, matrix mat00 through mat32: 6-17

```pascal
PROCEDURE SetTexMapReal(
				h        : HANDLE;
				partID   : LONGINT;
				selector : INTEGER;
				value    : REAL);
```

```python

def vs.SetTexMapReal(h, partID, selector, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|partID|LONGINT||
|selector|INTEGER||
|value|REAL||

## Version
```diff
- SetTexMapReal is obsolete as of Vectorworks 2010
```

Availability: from Vectorworks 2009
## Category
* Textures


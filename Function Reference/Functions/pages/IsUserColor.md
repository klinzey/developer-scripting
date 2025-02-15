# IsUserColor

## Description
Returns True if the color is a user color.

```pascal
FUNCTION IsUserColor(
				ColorIDX      : INTEGER;
				VAR ColorName : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.IsUserColor(ColorIDX):
    return (BOOLEAN, ColorName)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|ColorIDX|INTEGER||
|ColorName|DYNARRAY[] of CHAR||

## Remarks
ColorName returns the name of the color associated with the ColorIDX

## Version
Availability: from VectorWorks 2008
## Category
* Document Attributes


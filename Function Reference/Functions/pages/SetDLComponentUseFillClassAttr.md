# SetDLComponentUseFillClassAttr

## Description
Sets the use fill class attributes flag of the component at index in the Double Line Preferences.

```pascal
FUNCTION SetDLComponentUseFillClassAttr(
				index        : INTEGER;
				useClassAttr : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetDLComponentUseFillClassAttr(index, useClassAttr):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|useClassAttr|BOOLEAN|Whether or not the component will use class attributes for its fill.|

## See Also
VS Functions:
[GetDLComponentUseFillClassAttr](GetDLComponentUseFillClassAttr.md)

## Version
Availability: from VectorWorks 2008
## Category
* Document Settings


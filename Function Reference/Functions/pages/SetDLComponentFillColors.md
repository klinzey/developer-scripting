# SetDLComponentFillColors

## Description
Sets the fore and back fill colors of the component at index in the Double Line Preferences.

```pascal
FUNCTION SetDLComponentFillColors(
				index         : INTEGER;
				fillForeColor : INTEGER;
				fillBackColor : INTEGER) : BOOLEAN;
```

```python

def vs.SetDLComponentFillColors(index, fillForeColor, fillBackColor):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|fillForeColor|INTEGER|The fore color of the fill.|
|fillBackColor|INTEGER|The back color of the fill.|

## See Also
VS Functions:
[GetDLComponentFillColors](GetDLComponentFillColors.md)

## Version
Availability: from VectorWorks 2008
## Category
* Document Settings


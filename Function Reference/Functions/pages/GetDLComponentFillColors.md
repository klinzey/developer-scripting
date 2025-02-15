# GetDLComponentFillColors

## Description
Gets the fore and back fill colors of the component at index in the Double Line Preferences.

```pascal
FUNCTION GetDLComponentFillColors(
				index             : INTEGER;
				VAR fillForeColor : INTEGER;
				VAR fillBackColor : INTEGER) : BOOLEAN;
```

```python

def vs.GetDLComponentFillColors(index):
    return (BOOLEAN, fillForeColor, fillBackColor)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the component.|
|fillForeColor|INTEGER|Returns the fore color of the fill.|
|fillBackColor|INTEGER|Returns the back color of the fill.|

## See Also
VS Functions:
[SetDLComponentFillColors](SetDLComponentFillColors.md)

## Version
Availability: from VectorWorks 2008
## Category
* Document Settings


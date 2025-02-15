# SetClOpacity

## Description
Sets the opacity persentage of a class. The opacity is specified by percentage value in range [0-100].

```pascal
PROCEDURE SetClOpacity(
				className : STRING;
				opacity   : INTEGER);
```

```python

def vs.SetClOpacity(className, opacity):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|
|opacity|INTEGER|Opacity specified by percentage value in range [0-100].|

## Examples
```pascal
{set opacity of 25%}

SetClOpacity('Cold Water Supply',25);
```

## Version
Availability: from VectorWorks 2008
## Category
* Classes


# DimArcText

## Description
Procedure DimArcText creates an angular dimension object from the last arc object that was drawn using VectorScript.

```pascal
PROCEDURE DimArcText;
```

```python

def vs.DimArcText():
    return None
```

## Remarks
Creates an angular dimension object from the last arc object that was drawn using VectorScript

## Examples
```pascal
Arc(0,0,2,2,45d,90d);

DimArcText;

{ creates a dimension from the new arc object }
```

## Version
Availability: from MiniCAD
## Category
* Dimensions


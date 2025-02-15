# Rotate

## Description
Procedure Rotate rotates the currently selected objects on the active layer. The rotation angle may be specified in any valid angle format. When a locus is selected with a group of objects, the objects are rotated around the locus. If two or more loci are selected, the objects are rotated around the center of the selected objects.&lt;BR&gt;


```pascal
PROCEDURE Rotate(rotationAngle : REAL);
```

```python

def vs.Rotate(rotationAngle):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|rotationAngle|REAL|Rotation angle.|

## Examples
```pascal
Rotate(45d15'23&quot;);


```

## Version
Availability: from MiniCAD
## Category
* General Edit


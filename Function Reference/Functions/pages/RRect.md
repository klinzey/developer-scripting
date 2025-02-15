# RRect

## Description
Procedure RRect creates a rounded rectangle object in a Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
Corner definition is controlled by parameter Diam, which determines the &amp;quot;roundness&amp;quot; of the rectangle corners. The X and Y components of Diam correspond to the major and minor axes of an oval defining the rectangle corner.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE RRect(
				p1   : REAL;
				p2   : REAL;
				Diam : REAL);
```

```python

def vs.RRect(p1, p2, Diam):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Top left coordinate of rectangle.|
|p2|REAL|Bottom right coordinate of rectangle.|
|Diam|REAL|X and Y diameters of corner.|

## Examples
```pascal
PROCEDURE Example;

BEGIN

	RRect(0, 0, 1, 1, 0.25, 0.25);

	{same as: RRectangleN(0, 0, 1, 0, 1, 1, .25, .25);}

END;

RUN(Example);
```

## See Also
VS Functions:
[Rect](Rect.md)| [GetRRDiam](GetRRDiam.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


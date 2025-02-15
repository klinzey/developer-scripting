# Rect

## Description
Procedure Rect creates a rectangle object in a Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
The procedure will accept coordinate definitions by either of two methods : coordinate values or distance angle values. Coordinate values are the absolute coordinate locations(in the documents' coordinate system) and are expressed as x and y values. &lt;BR&gt;
&lt;BR&gt;
Distance-angle values are expressed as a distance and angle from the current pen position. For Rect, two distance angle pairs are required to specify the top left and bottom right of the rectangle object.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Rect(
				p1 : REAL;
				p2 : REAL);
```

```python

def vs.Rect(p1, p2):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Top left coordinate of rectangle.|
|p2|REAL|Bottom right coordinate of rectangle.|

## Examples
```pascal
Rect(0,2,2,1);

{creates a rectangle object by coordinate values}



Rect(0.5,#90,2,#0);

{creates a rectangle object by dist-angle values}


```

## See Also
VS Functions:
[RRect](RRect.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


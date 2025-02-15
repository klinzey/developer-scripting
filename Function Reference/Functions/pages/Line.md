# Line

## Description
Procedure Line creates a line object in Vectorworks. The line is drawn from the current pen position(x,y) to the specified point. The point may also be thought of as the location (x+dX,y+dY), where dX and dY are x and y offsets, respectively. &lt;BR&gt;
&lt;BR&gt;
The line object is drawn with the current default attributes unless otherwise specified.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Line(line : REAL);
```

```python

def vs.Line(line):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|line|REAL|Offset values for line.|

## Examples
```pascal
Line(2,2);

{ draws a line from the current pen location to a point }

{ 2 horizontal and 2 vertical units away.               }
```

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


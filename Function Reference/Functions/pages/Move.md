# Move

## Description
Sets the position of the graphics pen in the Vectorworks document by moving a specified distance from the current pen location. &lt;BR&gt;
&lt;BR&gt;
Horizontal and vertical offsets from the initial location. The final position of the pen at a point whose coordinates are (x+moveDX, y+moveDY).&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Move(move : REAL);
```

```python

def vs.Move(move):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|move|REAL|X-Y offset distance.|

## Examples
```pascal
Move(6,1);

{ moves the graphics pen 6 units to the right }

{ and 1 unit up from the current position.    }
```

## See Also
VS Functions:
[MoveTo](MoveTo.md)

## Version
Availability: from MiniCAD
## Category
* Command


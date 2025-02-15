# MoveTo

## Description
Sets the position of the graphics pen in the Vectorworks document using absolute coordinate values. The parameter specifies the X-Y coordinate location where the pen should be moved.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE MoveTo(p : REAL);
```

```python

def vs.MoveTo(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|X-Y coordinate location.|

## Examples
```pascal
MoveTo(4,3);

{moves the graphics pen to (4,3)}
```

## See Also
VS Functions:
[Move](Move.md)

## Version
Availability: from MiniCAD
## Category
* Command


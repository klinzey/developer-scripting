# LineTo

## Description
Procedure LineTo creates a line object in the document. LineTo draws from the current graphics pen position to the specified coordinate location. The line object is drawn with the current default attributes unless otherwise specified in the VectorScript routine.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE LineTo(p : REAL);
```

```python

def vs.LineTo(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Line endpoint.|

## Examples
```pascal
LineTo(3,4);

{draws a line from the current pen position to (3,4)}


```

## See Also
VS Functions:
[Absolute](Absolute.md)| [Relative](Relative.md)

## Version
Availability: from MiniCAD
## Category
* Objects - 2D


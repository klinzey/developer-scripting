# MouseDown

## Description
Function MouseDown returns TRUE if a mouse down event has occurred within the active document window.&lt;BR&gt;


```pascal
FUNCTION MouseDown(VAR p : REAL) : BOOLEAN;
```

```python

def vs.MouseDown():
    return (BOOLEAN, p)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Returns coordinates of mouse click.|

## Examples
```pascal
REPEAT

UNTIL MouseDown(x1,y1);

REPEAT

UNTIL MouseDown(x2,y2);

MoveTo(x1,y1);

LineTo(x2,y2);


```

## Version
Availability: from MiniCAD
## Category
* User Interactive


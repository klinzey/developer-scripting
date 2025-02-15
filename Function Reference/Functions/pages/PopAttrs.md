# PopAttrs

## Description
Restores the attribute, tool, and constraint settings saved by an earlier call to PushAttrs.&lt;BR&gt;


```pascal
PROCEDURE PopAttrs;
```

```python

def vs.PopAttrs():
    return None
```

## Examples
```pascal
PROCEDURE Example;

BEGIN

  PushAttrs;

  PenFore(215);

  PenBack(5);

  PenPat(25);

  PenSize(42);

  PenPat(25);

  SetConstrain('q');

  CallTool(-201);

  PopAttrs;

END;

RUN(Example);
```

## See Also
VS Functions:
[PushAttrs](PushAttrs.md)

## Version
Availability: from MiniCAD4.0
## Category
* Command


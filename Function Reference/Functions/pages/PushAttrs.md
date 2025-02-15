# PushAttrs

## Description
Stores current attribute, tool, text, and constraint settings for later retrieval as the document default settings. Document settings can be modified as needed after using this call, and the stored settings can be restored with a call to PopAttrs.  Calling this function more than once (nested) is allowed.  The settings will be placed on a stack, and will be retrieved by calls to PopAttrs in the correct sequence. &lt;BR&gt;


```pascal
PROCEDURE PushAttrs;
```

```python

def vs.PushAttrs():
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
[PopAttrs](PopAttrs.md)

## Version
Availability: from MiniCAD4.0
## Category
* Command


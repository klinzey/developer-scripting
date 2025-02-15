# BeginContext

## Description
Use this function in conjuction with EndContext to starts logging changes that are  made until the EndContext is reached.

```pascal
PROCEDURE BeginContext;
```

```python

def vs.BeginContext():
    return None
```

## Remarks
If you do not use this construct and you create a temporary plug-in object that itself creates a new class, the new class will remain even after you delete the temporary plug-in object.

## See Also
VS Functions:
[EndContext](EndContext.md)

## Version
Availability: from VectorWorks12.5
## Category
* Utility


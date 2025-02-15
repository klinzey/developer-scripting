# ActSymDef

## Description
Function ActSymDef returns a handle to the currently active symbol.&lt;BR&gt;
&lt;BR&gt;
If the active symbol is not in the active document, it will be imported, and the imported symbol will be returned.

```pascal
FUNCTION ActSymDef : HANDLE;
```

```python

def vs.ActSymDef():
    return HANDLE
```

## Examples
```pascal
HandleToActiveSym:=ActSymDef;
```

## See Also
VS Functions:
[ActLayer](ActLayer.md)| [ActiveClass](ActiveClass.md)| [ActSymDefN](ActSymDefN.md)

## Version
Availability: from MiniCAD
## Category
* Objects - Symbols


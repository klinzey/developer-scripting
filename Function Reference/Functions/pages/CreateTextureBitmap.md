# CreateTextureBitmap

## Description
Function CreateTextureBitmap creates a new default texture bitmap in a Vectorworks document.

```pascal
FUNCTION CreateTextureBitmap : HANDLE;
```

```python

def vs.CreateTextureBitmap():
    return HANDLE
```

## Remarks
Creates a new default texture bitmap, with no paint node attached.  Texture bitmap's paint node should be attached before this texture bitmap is used by MiniCAD (SetTexBitPaintNode).

## Version
```diff
- CreateTextureBitmap is obsolete as of VectorWorks10.1
```

Availability: from VectorWorks8.0
## Category
* Textures


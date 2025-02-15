# InsertNewComponent

## Description
Deprecated - will generate error. Use InsertNewComponentN instead.

```pascal
FUNCTION InsertNewComponent(
				object               : HANDLE;
				beforeComponentIndex : INTEGER;
				width                : REAL (Coordinate);
				fill                 : LONGINT;
				leftPenWeight        : INTEGER;
				rightPenWeight       : INTEGER;
				leftPenStyle         : INTEGER;
				rightPenStyle        : INTEGER) : BOOLEAN;
```

```python

def vs.InsertNewComponent(object, beforeComponentIndex, width, fill, leftPenWeight, rightPenWeight, leftPenStyle, rightPenStyle):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|object|HANDLE|The object. Can be a wall, round wall, slab, roof face, roof, Wall Style, Slab Style, Roof Style, the Wall Preferences, the Slab Preferences, or the Roof Preferences.|
|beforeComponentIndex|INTEGER|The index before which to insert the new component.|
|width|REAL (Coordinate)|The width of the component.|
|fill|LONGINT|The fill of the component.  Positive values for patterns, negative ref numbers for hatches.|
|leftPenWeight|INTEGER|The pen weight of the component's left line.|
|rightPenWeight|INTEGER|The pen weight of the component's right line.|
|leftPenStyle|INTEGER|The pen style of the component's left line.  Positive values for patterns, negative values for dash styles.|
|rightPenStyle|INTEGER|The pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use InsertNewComponentN instead.<BR>
The dash style it used no longer exists. Line types are used instead. Original description was: Inserts a new component in an object.

## See Also
VS Functions:
[InsertNewComponentN](InsertNewComponentN.md)

## Version
```diff
- InsertNewComponent is obsolete as of Vectorworks 2014
```

Availability: from VectorWorks12.0
## Category
* Objects - Architectural


# InsertNewDLComponent

## Description
Deprecated - will generate error. Use InsertNewDLCompN instead.

```pascal
FUNCTION InsertNewDLComponent(
				beforeIndex    : INTEGER;
				widthDistance  : REAL (Coordinate);
				fill           : LONGINT;
				penWeightLeft  : INTEGER;
				penWeightRight : INTEGER;
				penStyleLeft   : INTEGER;
				penStyleRight  : INTEGER) : BOOLEAN;
```

```python

def vs.InsertNewDLComponent(beforeIndex, widthDistance, fill, penWeightLeft, penWeightRight, penStyleLeft, penStyleRight):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|beforeIndex|INTEGER|The index before which to insert the new component.|
|widthDistance|REAL (Coordinate)|The width of the component.|
|fill|LONGINT|The fill of the component.  Positive values for patterns, negative ref numbers for hatches.|
|penWeightLeft|INTEGER|The pen weight of the component's left line.|
|penWeightRight|INTEGER|The pen weight of the component's right line.|
|penStyleLeft|INTEGER|The pen style of the component's left line.  Positive values for patterns, negative values for dash styles.|
|penStyleRight|INTEGER|The pen style of the component's right line.  Positive values for patterns, negative values for dash styles.|

## Remarks
Deprecated - will generate error. Use InsertNewDLCompN instead. The dash style it used no longer exists. Line types are used instead. Original description was: Inserts a new component before index in the Double Line Preferences.

## See Also
VS Functions:
[InsertNewDLCompN](InsertNewDLCompN.md)

## Version
```diff
- InsertNewDLComponent is obsolete as of Vectorworks 2019
```

Availability: from VectorWorks12.5
## Category
* Document Settings


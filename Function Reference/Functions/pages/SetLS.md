# SetLS

## Description
Deprecated - will generate error. Use SetLSN instead.

```pascal
PROCEDURE SetLS(
				h  : HANDLE;
				ls : INTEGER);
```

```python

def vs.SetLS(h, ls):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|ls|INTEGER|Linestyle to apply to object.|

## Remarks
Deprecated - will generate error. Use SetLSN instead. Original description was: Sets the linestyle of the referenced object. If the value is in the range 0 to 71, the specified fill pattern is applied as the linestyle; a value in the range of -1 to -8 will apply the specified linestyle.

## Examples
```pascal
PROCEDURE Example;

VAR

	cnt :INTEGER;

BEGIN

	PushAttrs;

	TextSize(1);

	TextJust(3);

	TextVerticalAlign(3);

	FOR cnt := -10 TO 71 DO BEGIN

		TextOrigin(-2, cnt);

		CreateText(Concat(cnt));

		MoveTo(0, cnt);

		LineTo(24&quot;, cnt);

		SetLS(LNewObj, cnt);

	END;

	PopAttrs;

END;

RUN(Example);
```

## See Also
VS Functions:
[SetLSN](SetLSN.md)

## Version
```diff
- SetLS is obsolete as of Vectorworks 2013
```

Availability: from MiniCAD
## Category
* Object Attributes


# SetTextWidth

## Description
Procedure SetTextWidth Sets the text wrapping margin width of the referenced text object.   &lt;BR&gt;
&lt;BR&gt;
A call to SetTextWidth automatically activates text wrapping.

```pascal
PROCEDURE SetTextWidth(
				theText       : HANDLE;
				widthDistance : REAL (Coordinate));
```

```python

def vs.SetTextWidth(theText, widthDistance):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theText|HANDLE|Handle to text object.|
|widthDistance|REAL (Coordinate)|Text wrapping margin setting for text.|

## Examples
```pascal
PROCEDURE Example;



FUNCTION IncreaseTextWidth(h :HANDLE) :BOOLEAN;

BEGIN

   SetTextWidth(h, GetTextWidth(h) * 1.2);

END;



BEGIN

   ForEachObjectInLayer(IncreaseTextWidth, 2, 0, 4);

END;

RUN(Example);


```

## See Also
VS Functions:
[GetTextWidth](GetTextWidth.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text


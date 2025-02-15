# GetTextOrientation

## Description
Procedure GetTextOrientation returns the position and orientation attributes of the referenced text object.

```pascal
PROCEDURE GetTextOrientation(
				theText            : HANDLE;
				VAR textOrigin     : REAL;
				VAR textAng        : REAL;
				VAR textIsMirrored : BOOLEAN);
```

```python

def vs.GetTextOrientation(theText):
    return (textOrigin, textAng, textIsMirrored)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theText|HANDLE|Handle to text object.|
|textOrigin|REAL|Returns coordinates of text origin.|
|textAng|REAL|Returns rotation angle of text.|
|textIsMirrored|BOOLEAN|Returns mirror state of text.|

## Examples
```pascal
PROCEDURE Example;

VAR

   theText :HANDLE;

   textOriginX, textOriginY, textAng :REAL;

   textIsMirrored :BOOLEAN;

BEGIN

   theText := FSActLayer;

   GetTextOrientation(theText, textOriginX, textOriginY, textAng, textIsMirrored);

   Locus(textOriginX, textOriginY);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Text


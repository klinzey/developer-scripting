# PenPatN

## Description
Procedure PenPatN sets the active pen pattern (line style) for the document. &lt;BR&gt;
&lt;BR&gt;
If patNumber is in the range 0 to 71 the linestyle will be set to the corresponding fill pattern. A negative value, will set the linestyle to the line type resource whose index is the negative of the value.

```pascal
PROCEDURE PenPatN(patNumber : LONGINT);
```

```python

def vs.PenPatN(patNumber):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|patNumber|LONGINT|Pattern/linestyle ID value.|

## Examples
```pascal
PenPat(25);

{ uses fill pattern 25 as the active pen pattern }



PenPat(-10);

{ sets the line type with the index of 10 as the active pen pattern }
```

## See Also
VS Functions:
[FPenPatN](FPenPatN.md)

## Version
Availability: from Vectorworks 2013
## Category
* Document Attributes


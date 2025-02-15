# SetLSN

## Description
Procedure SetLSN sets the linestyle of the referenced object.&lt;BR&gt;
&lt;BR&gt;
If the value is in the range 0 to 71, the specified fill pattern is applied as the linestyle; a negative value will apply the line type whose index is the negative of the value.

```pascal
PROCEDURE SetLSN(
				h  : HANDLE;
				ls : LONGINT);
```

```python

def vs.SetLSN(h, ls):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|ls|LONGINT|Linestyle to apply to object.|

## See Also
VS Functions:
[GetLSN](GetLSN.md)

## Version
Availability: from Vectorworks 2013
## Category
* Object Attributes


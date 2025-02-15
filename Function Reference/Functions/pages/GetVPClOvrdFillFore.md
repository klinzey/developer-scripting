# GetVPClOvrdFillFore

## Description
Fetches the fill foreground color of the class override. The color is returned as three RGB components in the range 0~65535.

```pascal
PROCEDURE GetVPClOvrdFillFore(
				viewportHandle : HANDLE;
				className      : STRING;
				VAR colorRV    : LONGINT;
				VAR colorGV    : LONGINT;
				VAR colorBV    : LONGINT);
```

```python

def vs.GetVPClOvrdFillFore(viewportHandle, className):
    return (colorRV, colorGV, colorBV)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE|The viewport handle.|
|className|STRING|The name of the class.|
|colorRV|LONGINT|Red color value.|
|colorGV|LONGINT|Green color value.|
|colorBV|LONGINT|Blue color value.|

## Returns
True if the viewport has an override for the specified class.<BR>
False if it does not have an override or the class or viewport was invalid.

## See Also
VS Functions:
[SetVPClOvrdFillFore](SetVPClOvrdFillFore.md)

## Version
Availability: from Vectorworks 2014
## Category
* Viewports


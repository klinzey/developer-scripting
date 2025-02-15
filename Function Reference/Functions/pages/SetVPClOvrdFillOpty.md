# SetVPClOvrdFillOpty

## Description
Sets the fill opacity for a viewport class override.

```pascal
PROCEDURE SetVPClOvrdFillOpty(
				viewportHandle : HANDLE;
				className      : STRING;
				fillOpacity    : INTEGER);
```

```python

def vs.SetVPClOvrdFillOpty(viewportHandle, className, fillOpacity):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE|The viewport handle.|
|className|STRING|Name of the class.|
|fillOpacity|INTEGER|The fill opacity as a percentage (0-100).|

## Returns
Returns true if the opacitiy could be set for the viewport override.<BR>
Returns false otherwise.

## Version
Availability: from Vectorworks 2014
## Category
* Viewports


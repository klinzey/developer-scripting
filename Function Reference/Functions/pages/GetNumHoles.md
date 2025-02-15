# GetNumHoles

## Description
Returns the number of openings in the referenced polyline.

```pascal
FUNCTION GetNumHoles(
				inPolyline      : HANDLE;
				VAR outNumHoles : INTEGER) : BOOLEAN;
```

```python

def vs.GetNumHoles(inPolyline):
    return (BOOLEAN, outNumHoles)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inPolyline|HANDLE|Handle to polyline.|
|outNumHoles|INTEGER|The number of openings in the polyline object.|

## Returns
Returns TRUE if the polyline contains openings, otherwise returns FALSE.

## See Also
VS Functions:
[GetHole](GetHole.md)

## Version
Availability: from VectorWorks9.0
## Category
* Objects - Polys


# SetSkylight

## Description
Function SetSkylight sets the definition attributes of a skylight in the referenced roof object.

```pascal
PROCEDURE SetSkylight(
				roofObject           : HANDLE;
				skylightID           : INTEGER;
				edgeIndex            : INTEGER;
				cornerOffsetDistance : REAL (Coordinate);
				perpOffsetDistance   : REAL (Coordinate);
				symName              : LONGINT);
```

```python

def vs.SetSkylight(roofObject, skylightID, edgeIndex, cornerOffsetDistance, perpOffsetDistance, symName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|roofObject|HANDLE|Handle to roof.|
|skylightID|INTEGER|Index of skylight element.|
|edgeIndex|INTEGER|Index of roof edge associated with skylight.|
|cornerOffsetDistance|REAL (Coordinate)|Offset of skylight from corner.|
|perpOffsetDistance|REAL (Coordinate)|Offset of skylight from roof edge.|
|symName|LONGINT|Name of skylight symbol.|

## Remarks
skylightID: Identifier for this skylight.  Value is returned by CreateSkylight().<BR>
edgeIndex: Index to which roof face this skylight is placed.  Value is one based.<BR>
cornerOffset: Top/Plan distance from vertex referenced by 'edgeIndex' to center of skylight.  This distance is parallel to the roof outline as defined by: vertex[edgeindex+1] - vertex[edgeIndex].<BR>
perpOffset: Top/Plan distance from roof outline to center of skylight.<BR>
symName: Skylight symbol to place in the roof.

## Examples
```pascal
skylightID:=CreateSkylight(roofHandle);

SetSkylight(roofHandle,skylightID,6,13'8&quot;,2'1&quot;,Name2Index('dh2436'));


```

## See Also
VS Functions:
[Name2Index](Name2Index.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Roofs


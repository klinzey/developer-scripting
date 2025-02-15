# OffsetPoly

## Description
Offsets a polygon or polyline. Must handle open &amp;amp; closed polys. A positive distance offsets to the outside; negative to the inside. Should remove self-intersecting segments from the result. Should support smooth vs. sharp offsets.

```pascal
FUNCTION OffsetPoly(
				h                      : HANDLE;
				offsetDistance         : REAL;
				numberOfOffsets        : INTEGER;
				consolidateVertices    : BOOLEAN;
				sharpCorners           : BOOLEAN;
				conversionRes          : INTEGER;
				consolidationTolerance : REAL) : HANDLE;
```

```python

def vs.OffsetPoly(h, offsetDistance, numberOfOffsets, consolidateVertices, sharpCorners, conversionRes, consolidationTolerance):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|offsetDistance|REAL||
|numberOfOffsets|INTEGER||
|consolidateVertices|BOOLEAN||
|sharpCorners|BOOLEAN||
|conversionRes|INTEGER||
|consolidationTolerance|REAL||

## Version
Availability: from Vectorworks 2014
## Category
* Graphic Calculation


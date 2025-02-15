# GetDashDataValPairAt

## Description
Deprecated - will generate error. Use GetDashDataValPrAtN instead.

```pascal
FUNCTION GetDashDataValPairAt(
				dashStyleIndex : INTEGER;
				dataIndex      : INTEGER;
				VAR dash       : REAL;
				VAR gap        : REAL) : BOOLEAN;
```

```python

def vs.GetDashDataValPairAt(dashStyleIndex, dataIndex):
    return (BOOLEAN, dash, gap)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dashStyleIndex|INTEGER|The dash style index.|
|dataIndex|INTEGER|Index fo the data value pair.|
|dash|REAL|The dash segement value.|
|gap|REAL|The gap segment value.|

## Remarks
Deprecated - will generate error. Use GetDashDataValPrAtN instead.

## Examples
```pascal
The dash-related functions here have been deprecated and will return errors. 

PROCEDURE Example;

VAR

n, numPairs, dashIndex : INTEGER;

scaleWThick  :BOOLEAN;

arrayDashDat : ARRAY[1..5] OF POINT;

x,y : REAL;



BEGIN



dashIndex := GetDashStyleIndex(TRUE, 2, 0.12, 0.18, 0.03, 0.07);



numPairs := GetNumDashDataPairs(dashIndex,scaleWThick);



FOR n := 1 TO numPairs DO BEGIN

 IF (GetDashDataValPairAt(dashIndex, n , x, y)) THEN BEGIN

   arrayDashDat[n].x := x ;

   arrayDashDat[n].y := y ;

 END; 

END;



END;

RUN(Example);
```

## See Also
VS Functions:
[GetDashDataValPrAtN](GetDashDataValPrAtN.md)

## Version
```diff
- GetDashDataValPairAt is obsolete as of Vectorworks 2019
```

Availability: from Vectorworks 2015
## Category
* Document Attributes


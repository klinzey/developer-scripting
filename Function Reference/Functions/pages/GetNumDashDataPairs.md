# GetNumDashDataPairs

## Description
Deprecated - will generate error. Use GetNumDashDataPairsN instead.

```pascal
FUNCTION GetNumDashDataPairs(
				dashIndex : INTEGER;
				VAR swt   : BOOLEAN) : INTEGER;
```

```python

def vs.GetNumDashDataPairs(dashIndex):
    return (INTEGER, swt)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dashIndex|INTEGER|The dash style index.|
|swt|BOOLEAN|The &quot;scale with thickness&quot; setting.|

## Remarks
Deprecated - will generate error. Use GetNumDashDataPairsN instead.

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
[GetNumDashDataPairsN](GetNumDashDataPairsN.md)

## Version
```diff
- GetNumDashDataPairs is obsolete as of Vectorworks 2019
```

Availability: from Vectorworks 2015
## Category
* Document Attributes


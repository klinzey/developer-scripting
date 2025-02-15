# GetDashStyleIndex

## Description
Deprecated - will generate error. Use GetDashStyleIndexN instead.

```pascal
FUNCTION GetDashStyleIndex(
				swt      : BOOLEAN;
				numPairs : INTEGER;
				pair1    : REAL;
				pair2    : REAL;
				pair3    : REAL;
				pair4    : REAL;
				pair5    : REAL) : INTEGER;
```

```python

def vs.GetDashStyleIndex(swt, numPairs, pair1, pair2, pair3, pair4, pair5):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|swt|BOOLEAN||
|numPairs|INTEGER||
|pair1|REAL||
|pair2|REAL||
|pair3|REAL||
|pair4|REAL||
|pair5|REAL||

## Remarks
Deprecated - will generate error. Use GetDashStyleIndexN instead.

## Examples
```pascal
GetDashStyleIndex(TRUE, 2, 0.12, 0.18, 0.03, 0.07);



GetDashStyleIndex(TRUE, 3, 0.12, 0.18, 0.03, 0.07, 0.2, 0.05);
```

## See Also
VS Functions:
[GetDashStyleIndexN](GetDashStyleIndexN.md)

## Version
```diff
- GetDashStyleIndex is obsolete as of Vectorworks 2019
```

Availability: from Vectorworks 2010
## Category
* Document Attributes


# GetNumGradientSegments

## Description
Gets the number of segments in the gradient.

```pascal
FUNCTION GetNumGradientSegments(gradient : HANDLE) : INTEGER;
```

```python

def vs.GetNumGradientSegments(gradient):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|gradient|HANDLE|The gradient from which to get the number of segments.|

## Returns
Returns the number of segments in the gradient if successful; 0 otherwise.

## Remarks
Note: a gradient must always have at least 2 segments.

## Examples
```pascal
numSegments := GetNumGradientSegments(gradientHandle);
```

## Version
Availability: from VectorWorks10.0
## Category
* Document Attributes


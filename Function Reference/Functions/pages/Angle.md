# Angle

## Description
Returns the angle value of a line segment or an arc. If more than one line segment or arc matches the search criteria, the function will return the sum of the matching objects' angle values.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION Angle(c : CRITERIA) : REAL;
```

```python

def vs.Angle(c):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|c|CRITERIA|Search criteria.|

## Returns
If an object matches the search criteria but is not a line segment or an arc, the value 0(zero) is returned.

## Examples
```pascal
aValue:=Angle(N='LineSeg');
```

## Version
Availability: from MiniCAD
## Category
* Criteria


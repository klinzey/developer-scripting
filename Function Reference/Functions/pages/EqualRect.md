# EqualRect

## Description
Function EqualRect returns whether the two specified rectangular areas are equal. &lt;BR&gt;


```pascal
FUNCTION EqualRect(
				rectAp1 : REAL;
				rectAp2 : REAL;
				rectBp1 : REAL;
				rectBp2 : REAL) : BOOLEAN;
```

```python

def vs.EqualRect(rectAp1, rectAp2, rectBp1, rectBp2):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|rectAp1|REAL|Top left coordinate of rectangle A.|
|rectAp2|REAL|Bottom right coordinate of rectangle A.|
|rectBp1|REAL|Top left coordinate of rectangle B.|
|rectBp2|REAL|Bottom right coordinate of rectangle B.|

## Examples
```pascal
AreTheyEqual:=EqualRect(0,0,3,3,3,3,0,0);


```

## Version
Availability: from MiniCAD
## Category
* Graphic Calculation


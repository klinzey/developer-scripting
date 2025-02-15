# Comp

## Description
Returns the components of a comparison of two vectors.&lt;BR&gt;
&lt;BR&gt;
The vector component of v1 along v2 in v3, and the vector component of v1 orthogonal to v2 in v4.&lt;BR&gt;


```pascal
PROCEDURE Comp(
				v1     : VECTOR;
				v2     : VECTOR;
				VAR v3 : VECTOR;
				VAR v4 : VECTOR);
```

```python

def vs.Comp(v1, v2, v3, v4):
    return (v3, v4)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v1|VECTOR|Comparison vector 1.|
|v2|VECTOR|Comparison vector 2|
|v3|VECTOR|Component of vector 1 along vector 2|
|v4|VECTOR|Component of vector 1 orthogonal to vector 2.|

## Version
Availability: from MiniCAD
## Category
* Math - Vectors


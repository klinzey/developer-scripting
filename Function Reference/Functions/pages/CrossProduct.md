# CrossProduct

## Description
Returns the cross product of the two specified vectors.&lt;BR&gt;
&lt;BR&gt;
The cross product is also known as the vector product of the two vectors. The result is a vector whose magnitude is equivalent to the product of the magnitudes of the two vectors multiplied by the sine of the smaller angle between the two vectors. The direction of the resultant vector is perpendicular to a plane formed by the two source vectors.

```pascal
FUNCTION CrossProduct(
				v1 : VECTOR;
				v2 : VECTOR) : VECTOR;
```

```python

def vs.CrossProduct(v1, v2):
    return VECTOR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v1|VECTOR|Source vector 1.|
|v2|VECTOR|Source vector 2.|

## Returns
Returns a VECTOR which is the cross product of v1 and v2.

## Remarks
This is provided for cross-platform compatibility.

## Version
Availability: from VectorWorks8.5
## Category
* Math - Vectors


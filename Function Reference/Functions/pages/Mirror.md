# Mirror

## Description
Reflect an object across an axis.&lt;BR&gt;
&lt;BR&gt;
For a 2D reflection, the axis is a line containing arbitrary point p and extending along vector v.

```pascal
FUNCTION Mirror(
				h   : HANDLE;
				dup : BOOLEAN;
				p1  : REAL;
				p2  : REAL) : HANDLE;
```

```python

def vs.Mirror(h, dup, p1, p2):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|The object to reflect|
|dup|BOOLEAN|If false, transform the original object to the new position. If true, create a new object|
|p1|REAL|An arbitrary point on the mirror axis|
|p2|REAL|A second arbitrary point on the mirror axis|

## Returns
The reflected object (this will be the same as the input object if dup is false).

## Version
Availability: from Vectorworks 2017
## Category
* Object Editing


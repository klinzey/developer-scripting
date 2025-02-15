# GetClosestPt

## Description
Returns the index number of the object closest to the specified location.  &lt;BR&gt;
&lt;BR&gt;
The index value will return 0 if no vertex can be determined as closest, and will return -1 if the object does not support GetClosestPt.&lt;BR&gt;
&lt;BR&gt;
For container objects, GetClosestPt has distinct behaviors. For walls, if the closest vertex is&lt;BR&gt;
is in a subobject, obj will be set to a handle to the subobject. For symbols and plug-in objects, an index to the sub-object will be returned via parameter containedObj.&lt;BR&gt;
&lt;BR&gt;
GetClosestPt supports only 2D objects.

```pascal
PROCEDURE GetClosestPt(
				VAR obj          : HANDLE;
				pt               : REAL;
				VAR index        : INTEGER;
				VAR containedObj : LONGINT);
```

```python

def vs.GetClosestPt(obj, pt):
    return (obj, index, containedObj)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|pt|REAL|Coordinate location of comparison point.|
|index|INTEGER|Index to vertex.|
|containedObj|LONGINT|Index of sub-object.|

## Examples
```pascal
PROCEDURE GetClosestPtExample;

VAR

	obj :HANDLE; 

	ptX, ptY :REAL; 

	index :INTEGER; 

	containedObj :LONGINT;

BEGIN

	GetPt(ptX, ptY);

	obj := PickObject(ptX, ptY);

	GetClosestPt(obj, ptX, ptY, index, containedObj);

	SetPenFore(obj, 65535, 0, 0);

END;

RUN(GetClosestPtExample);
```

## Version
Availability: from VectorWorks8.5
## Category
* Utility


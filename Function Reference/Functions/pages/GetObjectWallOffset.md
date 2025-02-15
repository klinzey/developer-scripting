# GetObjectWallOffset

## Description
Gets an object's offset value in it's break record. &lt;BR&gt;
&lt;BR&gt;
The object (objH) must be contained in wall (wallH)  to succeed.

```pascal
FUNCTION GetObjectWallOffset(
				objH       : HANDLE;
				wallH      : HANDLE;
				VAR offset : REAL) : BOOLEAN;
```

```python

def vs.GetObjectWallOffset(objH, wallH):
    return (BOOLEAN, offset)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE||
|wallH|HANDLE||
|offset|REAL||

## Returns
True or False upon successful setting of the flag.<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.

## Version
Availability: from Vectorworks 2015
## Category
* Objects - Walls


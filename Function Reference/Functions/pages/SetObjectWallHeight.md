# SetObjectWallHeight

## Description
Sets an object's height value in it's break record. &lt;BR&gt;
&lt;BR&gt;
The object (objH) must be contained in wall (wallH)  to succeed.

```pascal
FUNCTION SetObjectWallHeight(
				objH   : HANDLE;
				wallH  : HANDLE;
				height : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetObjectWallHeight(objH, wallH, height):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE||
|wallH|HANDLE||
|height|REAL (Coordinate)||

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


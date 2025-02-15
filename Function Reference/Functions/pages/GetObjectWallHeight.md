# GetObjectWallHeight

## Description
Gets an object's height value in it's break record. &lt;BR&gt;
&lt;BR&gt;
The object (objH) must be contained in wall (wallH)  to succeed.

```pascal
FUNCTION GetObjectWallHeight(
				objH       : HANDLE;
				wallH      : HANDLE;
				VAR height : REAL) : BOOLEAN;
```

```python

def vs.GetObjectWallHeight(objH, wallH):
    return (BOOLEAN, height)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE||
|wallH|HANDLE||
|height|REAL||

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


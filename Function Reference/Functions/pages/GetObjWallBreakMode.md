# GetObjWallBreakMode

## Description
Returns the break mode for an object in a wall.&lt;BR&gt;
&lt;BR&gt;
1 - Full Break with Caps&lt;BR&gt;
2 - Full Break no Caps&lt;BR&gt;
3 - Half Break&lt;BR&gt;
4 - No Break&lt;BR&gt;
&lt;BR&gt;
The object (objH) must be contained in wall (wallH)  to succeed.

```pascal
FUNCTION GetObjWallBreakMode(
				objH          : HANDLE;
				wallH         : HANDLE;
				VAR breakMode : INTEGER) : Boolean;
```

```python

def vs.GetObjWallBreakMode(objH, wallH, breakMode):
    return (Boolean, breakMode)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE||
|wallH|HANDLE||
|breakMode|INTEGER||

## Returns
True or False upon successful retrieving of the break mode.<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.

## Version
Availability: from Vectorworks 2017
## Category
* Objects - Walls


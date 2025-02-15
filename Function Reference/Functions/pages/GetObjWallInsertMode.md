# GetObjWallInsertMode

## Description
Returns the insertion mode for an object in a wall.&lt;BR&gt;
&lt;BR&gt;
0 - Insert on the center of the wall&lt;BR&gt;
1 - Insert on the left edge of the wall&lt;BR&gt;
2 - Insert on the right edge of the wall&lt;BR&gt;
3 - Insert on the center of the wall core component&lt;BR&gt;
4 - Insert on the left edge of the wall core component&lt;BR&gt;
5 - Insert on the right edge of the wall core component&lt;BR&gt;
&lt;BR&gt;
The object (objH) must be contained in wall (wallH)  to succeed.

```pascal
FUNCTION GetObjWallInsertMode(
				objH           : HANDLE;
				wallH          : HANDLE;
				VAR insertMode : INTEGER) : Boolean;
```

```python

def vs.GetObjWallInsertMode(objH, wallH, insertMode):
    return (Boolean, insertMode)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE||
|wallH|HANDLE||
|insertMode|INTEGER||

## Returns
True or False upon successful retrieving of the insertion mode.<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.

## Version
Availability: from Vectorworks 2017
## Category
* Objects - Walls


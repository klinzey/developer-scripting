# SetObjectAsSpanBreak

## Description
Sets an object's span wall flag in it's break record.&lt;BR&gt;
&lt;BR&gt;
Setting the flag to TRUE will force the object the center of the wall and set the offset position of the break record to reflect this.&lt;BR&gt;
&lt;BR&gt;
Setting the flag to FALSE will unset the span wall flag, but no further updating to the object will occur.&lt;BR&gt;
&lt;BR&gt;
The oject (objH) must be contained in wall (wallH) for the setting to succeed.

```pascal
FUNCTION SetObjectAsSpanBreak(
				objH          : HANDLE;
				wallH         : HANDLE;
				spanWallBreak : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetObjectAsSpanBreak(objH, wallH, spanWallBreak):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE|The handle of the object to update.|
|wallH|HANDLE|The handle of the wall cotainting the object referenced in objH.|
|spanWallBreak|BOOLEAN|Boolean value to set or unset the span wall  flag for the object.|

## Returns
True or False upon successfull setting of the flag<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.

## Version
Availability: from Vectorworks 2016
## Category
* Objects - Walls


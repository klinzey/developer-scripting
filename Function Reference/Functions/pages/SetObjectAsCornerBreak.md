# SetObjectAsCornerBreak

## Description
Sets an object's corner break flag in it's corner break record. &lt;BR&gt;
&lt;BR&gt;
Setting the flag to TRUE will force the object into the closest end of the wall and set the offset position of the break record to reflect this.&lt;BR&gt;
&lt;BR&gt;
Setting the flag to FALSE will unset the corner flag, but no further updating to the object will occur.&lt;BR&gt;
&lt;BR&gt;
The oject (objH) must be contained in wall (wallH) for the setting to succeed.

```pascal
FUNCTION SetObjectAsCornerBreak(
				objH        : HANDLE;
				wallH       : HANDLE;
				cornerBreak : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetObjectAsCornerBreak(objH, wallH, cornerBreak):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE|The handle of the object to update.|
|wallH|HANDLE|The handle of the wall cotainting the object referenced in objH.|
|cornerBreak|BOOLEAN|Boolean value to set or unset the cornerBreak flag for the object.|

## Returns
True or False upon successfull setting of the flag.<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.<BR>


## Version
Availability: from Vectorworks 2010
## Category
* Objects - Walls


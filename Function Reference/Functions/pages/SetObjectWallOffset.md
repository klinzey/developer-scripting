# SetObjectWallOffset

## Description
Sets an object's offset value in it's  break record. &lt;BR&gt;
&lt;BR&gt;
The oject (objH) must be contained in wall (wallH) for the setting to succeed.

```pascal
FUNCTION SetObjectWallOffset(
				objH   : HANDLE;
				wallH  : HANDLE;
				offset : REAL (Coordinate)) : BOOLEAN;
```

```python

def vs.SetObjectWallOffset(objH, wallH, offset):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objH|HANDLE|Handle of object to set a new offset value for.|
|wallH|HANDLE|Handle of wall containing the object refernces in objH.|
|offset|REAL (Coordinate)|Value of new offset for object within wall.|

## Returns
True or False upon successfull setting of the flag.<BR>
<BR>
False can occur for the following conditions:<BR>
objH is null.<BR>
wallH is null.<BR>
objH is not contained in wallH.

## Version
Availability: from Vectorworks 2010
## Category
* Objects - Walls


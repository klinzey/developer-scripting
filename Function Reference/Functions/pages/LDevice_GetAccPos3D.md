# LDevice_GetAccPos3D

## Description
Returns the 3D position and rotation of the specified accessory.

```pascal
PROCEDURE LDevice_GetAccPos3D(
				handle            : HANDLE;
				cellIndex         : LONGINT;
				accessoryIndex    : LONGINT;
				VAR outRotation3D : REAL;
				VAR outRotationX  : REAL;
				VAR outRotationY  : REAL;
				VAR outRotationZ  : REAL);
```

```python

def vs.LDevice_GetAccPos3D(handle, cellIndex, accessoryIndex):
    return (outRotation3D, outRotationX, outRotationY, outRotationZ)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|handle|HANDLE||
|cellIndex|LONGINT||
|accessoryIndex|LONGINT||
|outRotation3D|REAL||
|outRotationX|REAL||
|outRotationY|REAL||
|outRotationZ|REAL||

## Version
Availability: from Vectorworks 2021
## Category
* Spotlight


# CreateCustomObject

## Description
Creates a custom object instance at the specified location and angle of rotation. For the objectName, use the &amp;quot;internal&amp;quot; plug-in name (the one assigned in the plug-in editor), as opposed to the filename (which can be different).&lt;BR&gt;


```pascal
FUNCTION CreateCustomObject(
				objectName    : STRING;
				p             : REAL;
				rotationAngle : REAL) : HANDLE;
```

```python

def vs.CreateCustomObject(objectName, p, rotationAngle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectName|STRING|Name of object.|
|p|REAL|Insertion point of object instance.|
|rotationAngle|REAL|Rotation angle (in degrees) of object instance.|

## Returns
Returns a HANDLE to the new object.

## See Also
VS Functions:
[CreateCustomObjectPath](CreateCustomObjectPath.md)

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Custom


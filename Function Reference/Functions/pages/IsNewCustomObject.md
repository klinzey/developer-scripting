# IsNewCustomObject

## Description
Function IsNewCustomObject returns whether the specified plug-in object is a new object, indicating that the object is being regenerated for the first time.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
New object status is useful in specifying initialization and setup data, as well as calling initialization specific subroutines. This function should only be called in plug-in objects.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION IsNewCustomObject(objectName : STRING) : BOOLEAN;
```

```python

def vs.IsNewCustomObject(objectName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectName|STRING|Name of plugin object.|

## Remarks
Call from CustomObject scripts only.  Returns true for new objects, meaning this is the first time the regeneration script is being called.

## See Also
VS Functions:
[GetCustomObjectInfo](GetCustomObjectInfo.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Custom


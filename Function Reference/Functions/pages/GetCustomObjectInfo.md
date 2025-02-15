# GetCustomObjectInfo

## Description
Function GetCustomObjectInfo is used within plug-in object scripts to determine information about the object. Only returns false if the object is corrupt.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetCustomObjectInfo(
				VAR objectName : STRING;
				VAR objectHand : HANDLE;
				VAR recordHand : HANDLE;
				VAR wallHand   : HANDLE) : BOOLEAN;
```

```python

def vs.GetCustomObjectInfo():
    return (BOOLEAN, objectName, objectHand, recordHand, wallHand)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectName|STRING|Returns the name of the object.|
|objectHand|HANDLE|Returns a handle to the plugin object in the drawing.|
|recordHand|HANDLE|Returns a handle to the record containing current parameter values.|
|wallHand|HANDLE|Returns a handle to a wall, (if this object is in a wall). |

## Remarks
[sd 8/19/98]

## See Also
VS Functions:
[IsNewCustomObject](IsNewCustomObject.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Custom


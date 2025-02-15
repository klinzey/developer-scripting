# IsPluginFormat

## Description
Determines if the format node is used for the parameters of a plug-in object, plug-in tool or plug-in menu command.  

```pascal
FUNCTION IsPluginFormat(theFormat : HANDLE) : BOOLEAN;
```

```python

def vs.IsPluginFormat(theFormat):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theFormat|HANDLE|Handle to the format node in question.|

## Returns
Returns true if format is used by a plug-in and false if it is a regular format that may have been created by the user.

## Version
Availability: from VectorWorks11.0
## Category
* Objects - Custom


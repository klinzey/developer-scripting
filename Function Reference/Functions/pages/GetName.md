# GetName

## Description
Function GetName returns the object name of the referenced object. The function returns None if the object has no object name.&lt;BR&gt;
&lt;BR&gt;
A handle to layer may not passed to this routine; to obtain a layer name, use GetLName.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetName(h : HANDLE) : STRING;
```

```python

def vs.GetName(h):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
ObjectName:=GetName(HandleToObject);


```

## See Also
VS Functions:
[SetName](SetName.md)

## Version
Availability: from MiniCAD
## Category
* Object Names


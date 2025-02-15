# GetClass

## Description
Function GetClass returns the class assigned to the referenced object. None is returned if the object has no class assigned to it.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetClass(h : HANDLE) : STRING;
```

```python

def vs.GetClass(h):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
ObjectClass:=GetClass(handleToObject);
```

## Version
Availability: from MiniCAD
## Category
* Object Attributes


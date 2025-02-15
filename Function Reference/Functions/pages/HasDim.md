# HasDim

## Description
Function HasDim returns TRUE if a line or arc object has dimension text associated with it, otherwise it returns FALSE.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION HasDim(h : HANDLE) : BOOLEAN;
```

```python

def vs.HasDim(h):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
isDimension:=HasDim(HandleToObject);


```

## Version
Availability: from MiniCAD
## Category
* Dimensions


# NextObj

## Description
Function NextObj returns the next object in any list . If the end of the list is reached, the function returns NIL. This procedure can be used with other handle routines such as FirstIn3D,FInGroup, FirstInSymDef, or FLayer.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION NextObj(h : HANDLE) : HANDLE;
```

```python

def vs.NextObj(h):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object,  group, or  symbol definition.|

## Examples
```pascal
handleToObject:=FObject;

WHILE handleToObject &lt;&gt; NIL DO BEGIN

  i:=i+1;

  handleToObject:=NextObj(handleToObject);

END;


```

## Version
Availability: from MiniCAD
## Category
* Document List Handling


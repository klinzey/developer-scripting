# NextLayer

## Description
Function NextLayer returns a handle to the next layer in the document after the referenced. If the end of the list has been reached, the function returns NIL.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION NextLayer(h : HANDLE) : HANDLE;
```

```python

def vs.NextLayer(h):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to layer.|

## Examples
```pascal
handleToLayer:=FLayer;

WHILE handleToLayer &lt;&gt; NIL DO BEGIN

  SysBeep;

  handleToLayer:=NextLayer(handleToLayer);

END; 

{ will process through all the layers in the list }
```

## Version
Availability: from MiniCAD
## Category
* Document List Handling


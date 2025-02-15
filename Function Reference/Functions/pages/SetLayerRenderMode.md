# SetLayerRenderMode

## Description
Sets the render mode of the referenced layer.

```pascal
PROCEDURE SetLayerRenderMode(
				theLayer      : HANDLE;
				newRenderMode : INTEGER;
				immediate     : BOOLEAN;
				doProgress    : BOOLEAN);
```

```python

def vs.SetLayerRenderMode(theLayer, newRenderMode, immediate, doProgress):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theLayer|HANDLE|Handle of the layer|
|newRenderMode|INTEGER|New render mode to set|
|immediate|BOOLEAN|If true, then all rendering will take place before the call returns. Otherwise, any rendering that can take place in the background will be postponed until program execution re-enters the main event loop|
|doProgress|BOOLEAN|controls whether progress information is displayed during the operation|

## Version
Availability: from VectorWorks10.0
## Category
* Layers


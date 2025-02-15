# IsLayerReferenced

## Description
Returns whether a layer is workgroup referenced, and if so, the path to the source document is returned.

```pascal
FUNCTION IsLayerReferenced(
				layer        : HANDLE;
				VAR pathname : STRING) : BOOLEAN;
```

```python

def vs.IsLayerReferenced(layer):
    return (BOOLEAN, pathname)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|layer|HANDLE|Handle to the layer|
|pathname|STRING|On return, a string containing the path to the source document|

## Returns
Returns true if the layer is referenced, false otherwise.

## Version
Availability: from VectorWorks10.0
## Category
* Layers


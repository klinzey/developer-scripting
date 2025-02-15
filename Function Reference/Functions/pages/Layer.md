# Layer

## Description
Procedure Layer creates a new layer in a Vectorworks document. After creation, the new layer becomes the active layer of the document.&lt;BR&gt;
&lt;BR&gt;
Layer can also be used to switch the active layer of the document. If the layer name passed to the procedure already exists, the procedure switches the active layer to the specified layer.&lt;BR&gt;
&lt;BR&gt;
Single quotes should be avoided in layer names, as they will be treated as a mismatched string specifier, and will cause an error to be generated.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Layer(name : STRING);
```

```python

def vs.Layer(name):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|Name of new or existing layer.|

## Examples
```pascal
Layer('Ductwork-1st Floor');

{creates a new layer named 'Ductwork-1st Floor'}



Layer(newLayerName);

{creates a new layer whose name is specified in the variable}



Layer('Untitled-1');

{switches to the existing layer 'Untitled-1'}
```

## Version
Availability: from MiniCAD
## Category
* Layers


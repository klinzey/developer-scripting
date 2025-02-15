# CreateLayer

## Description
Creates a layer of the specified type.&lt;BR&gt;
&lt;BR&gt;
layerType values:&lt;BR&gt;
Design = 1&lt;BR&gt;
Presentation	= 2&lt;BR&gt;


```pascal
FUNCTION CreateLayer(
				layerName : STRING;
				layerType : INTEGER) : HANDLE;
```

```python

def vs.CreateLayer(layerName, layerType):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|layerName|STRING||
|layerType|INTEGER||

## Version
Availability: from VectorWorks10.5
## Category
* Layers


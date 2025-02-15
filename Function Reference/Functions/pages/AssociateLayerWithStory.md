# AssociateLayerWithStory

## Description
Associates a Layer with a Story. When a Layer is associated with a Story, the Layer's elevation is displayed relative to the Story elevation. If the elevation of the associated Story is changed, the elevation of the Layer changes with it.

```pascal
FUNCTION AssociateLayerWithStory(
				layer : HANDLE;
				story : HANDLE) : BOOLEAN;
```

```python

def vs.AssociateLayerWithStory(layer, story):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|layer|HANDLE|The Layer to associate.|
|story|HANDLE|The Story to associate.|

## Returns
Whether the Layer was successfully associated with the Story. This will fail if there is already another Layer associated with the Story that has the same Layer Level Type as the Layer passed in.

## Examples
```pascal
VAR



success:BOOLEAN;

story:HANDLE;

layer:HANDLE;



BEGIN



story := GetObject('4th Floor');

layer := GetObject('Plan 4');

success := AssociateLayerWithStory(layer, story);


```

## See Also
VS Functions:
[GetNumStories](GetNumStories.md)| [GetStoryOfLayer](GetStoryOfLayer.md)| [CreateStory](CreateStory.md)

## Version
Availability: from Vectorworks 2012
## Category
* Layers


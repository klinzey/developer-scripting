# DeleteLevelTemplate

## Description
Deletes the nth Story Level Template from the current file. For example, if 3 is passed in, it will delete the 3rd Story Level Template in the file. 

```pascal
FUNCTION DeleteLevelTemplate(index : INTEGER) : BOOLEAN;
```

```python

def vs.DeleteLevelTemplate(index):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the Story Level Template to be deleted.|

## Returns
Whether the Story Level Template at 'index' was found and deleted successfully.

## Examples
```pascal
VAR



success:BOOLEAN;



BEGIN



success := DeleteStoryTemplate(3);
```

## See Also
VS Functions:
[GetNumStoryLayerTemplates](GetNumStoryLayerTemplates.md)| [GetLevelTemplateName](GetLevelTemplateName.md)| [SetLevelTemplateName](SetLevelTemplateName.md)| [CreateLevelTemplate](CreateLevelTemplate.md)| [GetLevelTemplateInfo](GetLevelTemplateInfo.md)

## Version
Availability: from Vectorworks 2015
## Category
* Layers


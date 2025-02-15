# ResetDefStoryLevels

## Description
Clears default story levels and repopulates the list from XML data files on disk.

```pascal
FUNCTION ResetDefStoryLevels(bDeleteExisting : BOOLEAN) : BOOLEAN;
```

```python

def vs.ResetDefStoryLevels(bDeleteExisting):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|bDeleteExisting|BOOLEAN|Whether to delete existing default story levels before reloading the original defaults.|

## Returns
Whether clearing the previous default story levels and loading the default list from disk succeeded.

## See Also
VS Functions:
[GetLevelTemplateName](GetLevelTemplateName.md)| [SetLevelTemplateName](SetLevelTemplateName.md)| [GetLevelTemplateInfo](GetLevelTemplateInfo.md)| [GetNumLevelTemplates](GetNumLevelTemplates.md)

## Version
Availability: from Vectorworks 2015
## Category
* Layers


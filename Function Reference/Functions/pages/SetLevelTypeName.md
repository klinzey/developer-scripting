# SetLevelTypeName

## Description
Sets the name of the nth Level Type in the file. For example, if 3 is passed in, it will set the name of the 3rd Level Type in the file.

```pascal
FUNCTION SetLevelTypeName(
				index : INTEGER;
				name  : STRING) : BOOLEAN;
```

```python

def vs.SetLevelTypeName(index, name):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|The index of the level type whose name is being set.|
|name|STRING|The name the indicated level type should be set to.|

## Returns
Whether the setting of the name of the level type succeeded. It will fail if passed an invalid index. The name must not have more than 63 characters and must not be used by another level type in the file.

## Examples
```pascal
VAR



result : BOOLEAN;



BEGIN



result := SetLayerLevelTypeName(2, &quot;Subfloor&quot;);
```

## See Also
VS Functions:
[GetNumLayerLevelTypes](GetNumLayerLevelTypes.md)| [GetLevelTypeName](GetLevelTypeName.md)

## Version
Availability: from Vectorworks 2013
## Category
* Layers


# Rpstr_GetValueBool

## Description
Get a boolean value from the VectorScript value repository.

```pascal
FUNCTION Rpstr_GetValueBool(
				name         : STRING;
				defaultValue : BOOLEAN) : BOOLEAN;
```

```python

def vs.Rpstr_GetValueBool(name, defaultValue):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|The name of the value.|
|defaultValue|BOOLEAN|Default value if the name does not exist in the VectorScript value repository.|

## See Also
VS Functions:
[Rpstr_RemoveValues](Rpstr_RemoveValues.md)| [Rpstr_RemoveValue](Rpstr_RemoveValue.md)| [Rpstr_GetValueBool](Rpstr_GetValueBool.md)| [Rpstr_SetValueBool](Rpstr_SetValueBool.md)| [Rpstr_GetValueInt](Rpstr_GetValueInt.md)| [Rpstr_SetValueInt](Rpstr_SetValueInt.md)| [Rpstr_GetValueReal](Rpstr_GetValueReal.md)| [Rpstr_SetValueReal](Rpstr_SetValueReal.md)| [Rpstr_GetValueStr](Rpstr_GetValueStr.md)| [Rpstr_SetValueStr](Rpstr_SetValueStr.md)

## Version
Availability: from Vectorworks 2012
## Category
* Utility


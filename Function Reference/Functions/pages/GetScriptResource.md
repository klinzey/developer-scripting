# GetScriptResource

## Description
Return the script text of the specified script resource.

```pascal
FUNCTION GetScriptResource(
				scriptName : STRING;
				VAR script : DYNARRAY[] of CHAR;
				VAR python : BOOLEAN) : BOOLEAN;
```

```python

def vs.GetScriptResource(scriptName):
    return (BOOLEAN, script, python)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|scriptName|STRING|The script name identifying the resource.|
|script|DYNARRAY[] of CHAR|Return the script text.|
|python|BOOLEAN|Return if the script text is a python script.|

## Returns
Return TRUE if the creation was successful. The routine will fail if script with the specified name does't exist.

## See Also
VS Functions:
[CreateScriptResource](CreateScriptResource.md)| [SetScriptResource](SetScriptResource.md)| [OpenScriptResPal](OpenScriptResPal.md)

## Version
Availability: from Vectorworks 2014
## Category
* General Edit


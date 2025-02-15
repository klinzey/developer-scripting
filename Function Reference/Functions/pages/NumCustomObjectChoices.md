# NumCustomObjectChoices

## Description
Function NumCustomObjectChoices returns the number of choice strings for a specified popup menu or radio group parameter in a plug-in object. &lt;BR&gt;
&lt;BR&gt;
The string passed into the parameter name argument should use the parameter constant syntax, not the actual parameter name.  The string should have the prefix character 'P', and should have all spaces replaced with underscore characters.  For example, a parameter Jamb Depth would have a constant declared as PJAMB_DEPTH and therefore the parameter name argument to this function should be the string 'PJAMB_DEPTH'.

```pascal
FUNCTION NumCustomObjectChoices(
				objectName    : STRING;
				parameterName : STRING) : INTEGER;
```

```python

def vs.NumCustomObjectChoices(objectName, parameterName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectName|STRING|Name of plugin object.|
|parameterName|STRING|String indicating which parameter|

## Remarks
Call from CustomObject scripts only.  Return number of choice strings for a particular popup menu or radio group parameter.

## Examples
```pascal
maxChoices := NumCustomObjectChoices(objName, 'PDINNER_MENU');
```

## See Also
VS Functions:
[GetCustomObjectChoice](GetCustomObjectChoice.md)

## Version
Availability: from VectorWorks8.0
## Category
* Objects - Custom


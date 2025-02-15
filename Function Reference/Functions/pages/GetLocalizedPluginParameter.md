# GetLocalizedPluginParameter

## Description
Get the localized name of a plug-in parameter.&lt;BR&gt;
&lt;BR&gt;
When Vectorworks plug-ins are localized by distributors in other countries, their parameter names are translated to the appropriate language.  The plug-in file stores both the original universal name and this translated localized name for each parameter.  The translated name is displayed by the Vectorworks user interface instead of the original name.  If a script needs to display the name of a plug-in parameter in a dialog or message then it should call this function to determine the localized name.  (Note that scripts will use the universal name to specify a plug-in parameter when the name is not being displayed to the user.) &lt;BR&gt;
&lt;BR&gt;
If the plug-in has not been localized, then this function will return the universal name of the parameter.

```pascal
FUNCTION GetLocalizedPluginParameter(
				inPluginName     : STRING;
				inParameterName  : STRING;
				VAR outParameter : STRING) : BOOLEAN;
```

```python

def vs.GetLocalizedPluginParameter(inPluginName, inParameterName):
    return (BOOLEAN, outParameter)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inPluginName|STRING|Universal name of the plug-in.|
|inParameterName|STRING|Universal name of the parameter.|
|outParameter|STRING|Localized name of the parameter.|

## Returns
Returns true if the specified plug-in exists, and false if it is not found.

## See Also
VS Functions:
[GetLocalizedPluginName](GetLocalizedPluginName.md)

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Custom


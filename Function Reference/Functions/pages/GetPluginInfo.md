# GetPluginInfo

## Description
Returns the name and attached parameter record of the currently executing plug-in. Use with menu command or tool item plug-ins.

```pascal
FUNCTION GetPluginInfo(
				VAR pluginName : STRING;
				VAR recordHand : HANDLE) : BOOLEAN;
```

```python

def vs.GetPluginInfo():
    return (BOOLEAN, pluginName, recordHand)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|pluginName|STRING|Name of plug-in.|
|recordHand|HANDLE|Handle to parameter record of plug-in.|

## Remarks
Maybe a new function class of &quot;Plug-ins&quot; would be more appropriate than &quot;Objects - Custom&quot;.

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Custom


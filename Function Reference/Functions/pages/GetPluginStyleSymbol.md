# GetPluginStyleSymbol

## Description
Retrieves the handled to a symbol that defines the plug-in style for a given plug-in object.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetPluginStyleSymbol(
				hObject     : HANDLE;
				VAR hSymDef : HANDLE) : BOOLEAN;
```

```python

def vs.GetPluginStyleSymbol(hObject, hSymDef):
    return (BOOLEAN, hSymDef)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE|Handle to a plug-in object.|
|hSymDef|HANDLE|Hanlde to a symbol definition that contrains the plug-in style associated with hObject.|

## Returns
TRUE if the object is styled.<BR>
FALSE if the object is uynstyled.

## Version
Availability: from Vectorworks 2017
## Category
* Objects - Custom


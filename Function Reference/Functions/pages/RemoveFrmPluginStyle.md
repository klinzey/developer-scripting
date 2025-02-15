# RemoveFrmPluginStyle

## Description
Removes an entry from the plug-in style map.

```pascal
FUNCTION RemoveFrmPluginStyle(
				hSymDef  : HANDLE;
				itemName : STRING) : BOOLEAN;
```

```python

def vs.RemoveFrmPluginStyle(hSymDef, itemName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hSymDef|HANDLE|Handle to symbol definition containing a plug-in style.|
|itemName|STRING|Name of the item to remove from the plug-in style.|

## Returns
TRUE if the item was removed from the plug-in style.<BR>
FALSE if the item does not exist in the plug-in style or the symbol definition does not contain a plugin style.

## Version
Availability: from Vectorworks 2017
## Category
* Objects - Symbols


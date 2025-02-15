# SelectPluginCatalog

## Description
Brings up a dialog to select a catalog to attach to a plug-in style, change the attached catalog, or detach the current catalog.

```pascal
FUNCTION SelectPluginCatalog(hSymbol : HANDLE) : BOOLEAN;
```

```python

def vs.SelectPluginCatalog(hSymbol):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hSymbol|HANDLE|Handle to a symbol the defines a plug-in style.|

## Returns
FALSE if the object is not a symbol, does not define a plug-in sytle, or does not support catalogs.

## Version
Availability: from Vectorworks 2018
## Category
* Objects - Custom


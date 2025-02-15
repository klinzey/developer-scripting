# IFC_GetPsetProp

## Description
Gets the value and type of a selected property from a property set

```pascal
FUNCTION IFC_GetPsetProp(
				hObject             : HANDLE;
				inStrPsetName       : STRING;
				inStrPropName       : STRING;
				VAR outStrPropValue : STRING;
				VAR outTypeSelect   : INTEGER) : BOOLEAN;
```

```python

def vs.IFC_GetPsetProp(hObject, inStrPsetName, inStrPropName):
    return (BOOLEAN, outStrPropValue, outTypeSelect)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE||
|inStrPsetName|STRING||
|inStrPropName|STRING||
|outStrPropValue|STRING||
|outTypeSelect|INTEGER||

## Version
Availability: from Vectorworks 2014
## Category
* IFC


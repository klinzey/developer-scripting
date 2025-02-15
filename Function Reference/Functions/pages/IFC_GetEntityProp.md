# IFC_GetEntityProp

## Description
Gets the value and type of a selected property from the IFC entity

```pascal
FUNCTION IFC_GetEntityProp(
				hObject             : HANDLE;
				inStrPropName       : STRING;
				VAR outStrPropValue : STRING;
				VAR outTypeSelect   : INTEGER) : BOOLEAN;
```

```python

def vs.IFC_GetEntityProp(hObject, inStrPropName):
    return (BOOLEAN, outStrPropValue, outTypeSelect)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE||
|inStrPropName|STRING||
|outStrPropValue|STRING||
|outTypeSelect|INTEGER||

## Version
Availability: from Vectorworks 2014
## Category
* IFC


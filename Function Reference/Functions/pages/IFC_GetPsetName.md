# IFC_GetPsetName

## Description
Gets the name of the property set at that index

```pascal
FUNCTION IFC_GetPsetName(
				hObject            : HANDLE;
				inPsetIndex        : INTEGER;
				VAR outStrPsetName : STRING) : BOOLEAN;
```

```python

def vs.IFC_GetPsetName(hObject, inPsetIndex):
    return (BOOLEAN, outStrPsetName)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE||
|inPsetIndex|INTEGER||
|outStrPsetName|STRING||

## Version
Availability: from Vectorworks 2014
## Category
* IFC


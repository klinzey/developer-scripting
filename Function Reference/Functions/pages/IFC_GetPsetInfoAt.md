# IFC_GetPsetInfoAt

## Description
Gets the Pset name and if it is attached and where from (if it is from mapping or from record).

```pascal
FUNCTION IFC_GetPsetInfoAt(
				hObject            : HANDLE;
				bAllPsets          : BOOLEAN;
				index              : INTEGER;
				VAR outIfcPsetName : STRING;
				VAR outType        : INTEGER) : BOOLEAN;
```

```python

def vs.IFC_GetPsetInfoAt(hObject, bAllPsets, index):
    return (BOOLEAN, outIfcPsetName, outType)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE||
|bAllPsets|BOOLEAN||
|index|INTEGER||
|outIfcPsetName|STRING||
|outType|INTEGER||

## Version
Availability: from Vectorworks 2018
## Category
* IFC


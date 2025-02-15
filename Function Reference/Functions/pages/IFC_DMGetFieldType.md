# IFC_DMGetFieldType

## Description
Gets indicated field type from current IFC Data Mapping.

```pascal
FUNCTION IFC_DMGetFieldType(
				inStrObjName   : STRING;
				inStrEntryName : STRING;
				inStrFieldName : STRING;
				VAR outType    : INTEGER) : BOOLEAN;
```

```python

def vs.IFC_DMGetFieldType(inStrObjName, inStrEntryName, inStrFieldName):
    return (BOOLEAN, outType)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inStrObjName|STRING||
|inStrEntryName|STRING||
|inStrFieldName|STRING||
|outType|INTEGER||

## Version
Availability: from Vectorworks 2017
## Category
* IFC


# IFC_GetEntityColor

## Description
Gets the default color for an IFC entity type

```pascal
FUNCTION IFC_GetEntityColor(
				inStrIfcType  : STRING;
				VAR outRed    : INTEGER;
				VAR outGreen  : INTEGER;
				VAR outBlue   : INTEGER;
				VAR outTransp : INTEGER) : BOOLEAN;
```

```python

def vs.IFC_GetEntityColor(inStrIfcType):
    return (BOOLEAN, outRed, outGreen, outBlue, outTransp)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inStrIfcType|STRING||
|outRed|INTEGER||
|outGreen|INTEGER||
|outBlue|INTEGER||
|outTransp|INTEGER||

## Version
Availability: from Vectorworks 2014
## Category
* IFC


# HasPlugin

## Description
Returns whether tool item or menu command is in current workspace.

```pascal
FUNCTION HasPlugin(
				itemUniversalName : STRING;
				VAR PaletteName   : STRING) : BOOLEAN;
```

```python

def vs.HasPlugin(itemUniversalName):
    return (BOOLEAN, PaletteName)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|itemUniversalName|STRING|Universal name of the plug-in|
|PaletteName|STRING|If plug-in is a tool, and is found in the workspace, the name of the palette in which it is contained will be returned in this parameter|

## Returns
Returns true if the plug-in is found in the workspace; false otherwise.

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Custom


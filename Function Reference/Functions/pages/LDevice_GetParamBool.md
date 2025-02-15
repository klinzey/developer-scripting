# LDevice_GetParamBool

## Description
Get boolean parameter of a Lighting Device or attached Accessory by Worksheet Name. Use cell index 0 to operate on the first cell. Use accessory index -1 to access the ligting device parameters.

```pascal
FUNCTION LDevice_GetParamBool(
				handle         : HANDLE;
				cellIndex      : LONGINT;
				accessoryIndex : LONGINT;
				universalName  : STRING) : BOOLEAN;
```

```python

def vs.LDevice_GetParamBool(handle, cellIndex, accessoryIndex, universalName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|handle|HANDLE||
|cellIndex|LONGINT||
|accessoryIndex|LONGINT||
|universalName|STRING||

## Version
Availability: from Vectorworks 2021
## Category
* Spotlight


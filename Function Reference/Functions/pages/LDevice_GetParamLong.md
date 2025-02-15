# LDevice_GetParamLong

## Description
Get iong integer parameter of a Lighting Device or attached Accessory by Worksheet Name. Use cell index 0 to operate on the first cell. Use accessory index -1 to access the ligting device parameters.

```pascal
FUNCTION LDevice_GetParamLong(
				handle         : HANDLE;
				cellIndex      : LONGINT;
				accessoryIndex : LONGINT;
				universalName  : STRING) : LONGINT;
```

```python

def vs.LDevice_GetParamLong(handle, cellIndex, accessoryIndex, universalName):
    return LONGINT
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


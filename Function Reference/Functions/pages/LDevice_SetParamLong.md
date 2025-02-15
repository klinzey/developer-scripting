# LDevice_SetParamLong

## Description
Set iong integer parameter of a Lighting Device or attached Accessory by Worksheet Name. Use cell index 0 to operate on the first cell. Use accessory index -1 to access the ligting device parameters.

```pascal
PROCEDURE LDevice_SetParamLong(
				handle         : HANDLE;
				cellIndex      : LONGINT;
				accessoryIndex : LONGINT;
				universalName  : STRING;
				newValue       : LONGINT);
```

```python

def vs.LDevice_SetParamLong(handle, cellIndex, accessoryIndex, universalName, newValue):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|handle|HANDLE||
|cellIndex|LONGINT||
|accessoryIndex|LONGINT||
|universalName|STRING||
|newValue|LONGINT||

## Version
Availability: from Vectorworks 2021
## Category
* Spotlight


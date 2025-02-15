# LDevice_SetParamReal

## Description
Set real parameter of a Lighting Device or attached Accessory by Worksheet Name. Use cell index 0 to operate on the first cell. Use accessory index -1 to access the ligting device parameters.

```pascal
PROCEDURE LDevice_SetParamReal(
				handle         : HANDLE;
				cellIndex      : LONGINT;
				accessoryIndex : LONGINT;
				universalName  : STRING;
				newValue       : REAL);
```

```python

def vs.LDevice_SetParamReal(handle, cellIndex, accessoryIndex, universalName, newValue):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|handle|HANDLE||
|cellIndex|LONGINT||
|accessoryIndex|LONGINT||
|universalName|STRING||
|newValue|REAL||

## Version
Availability: from Vectorworks 2021
## Category
* Spotlight


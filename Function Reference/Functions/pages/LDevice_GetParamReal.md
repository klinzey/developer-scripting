# LDevice_GetParamReal

## Description
Get real parameter of a Lighting Device or attached Accessory by Worksheet Name. Use cell index 0 to operate on the first cell. Use accessory index -1 to access the ligting device parameters.

```pascal
FUNCTION LDevice_GetParamReal(
				handle         : HANDLE;
				cellIndex      : LONGINT;
				accessoryIndex : LONGINT;
				universalName  : STRING) : REAL;
```

```python

def vs.LDevice_GetParamReal(handle, cellIndex, accessoryIndex, universalName):
    return REAL
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


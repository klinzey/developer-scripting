# SetSavedSetting

## Description
Writes a value to the saved settings file.  This can be used to remember various user settings between running sessions of Vectorworks.  For example, a script may want to remember a dialog's position or a font settings.  The saved settings should not be used for critical information, but rather for convenience settings. 

```pascal
PROCEDURE SetSavedSetting(
				category : STRING;
				setting  : STRING;
				value    : STRING);
```

```python

def vs.SetSavedSetting(category, setting, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|category|STRING||
|setting|STRING||
|value|STRING||

## Version
Availability: from VectorWorks12.0
## Category
* Utility


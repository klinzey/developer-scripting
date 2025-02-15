# GetSavedSetting

## Description
Reads a value from the saved settnigs file.  This can be used to remember various user settings between running sessions of Vectorworks.  For example, a script may want to remember a dialog's position or a font settings.  The saved settings should not be used for critical information, but rather for convenience settings. &lt;BR&gt;
&lt;BR&gt;
If the settings file is lost or damaged the script should revert to a reasonable default value, and typically this would not warrant an alert dialog.

```pascal
FUNCTION GetSavedSetting(
				category  : STRING;
				setting   : STRING;
				VAR value : STRING) : BOOLEAN;
```

```python

def vs.GetSavedSetting(category, setting):
    return (BOOLEAN, value)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|category|STRING||
|setting|STRING||
|value|STRING||

## Returns
Returns true is the requested setting is found and read from the saved settings file, false otherwise.  

## Version
Availability: from VectorWorks12.0
## Category
* Utility


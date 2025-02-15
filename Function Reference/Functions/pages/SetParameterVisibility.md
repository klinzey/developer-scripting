# SetParameterVisibility

## Description
For plug-in objects, this procedure sets whether or not the specified parameter is visible on the Object Info Palette.  This routine is used inside plug-in object regeneration scripts to set their parameter visibility.  This visibility is an object instance property.

```pascal
PROCEDURE SetParameterVisibility(
				inPlugin        : HANDLE;
				inParameterName : STRING;
				inSetVisible    : BOOLEAN);
```

```python

def vs.SetParameterVisibility(inPlugin, inParameterName, inSetVisible):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inPlugin|HANDLE|Handle to the currently executing plug-in object.|
|inParameterName|STRING|Name of parameter, as it appears in the plug-in editor's parameter list.|
|inSetVisible|BOOLEAN|The new visibility state for the parameter specified. |

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Custom


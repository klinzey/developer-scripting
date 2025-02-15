# GetPluginString

## Description
Returns the string specified by stringIndex. The strings are created using the &amp;quot;Strings&amp;quot; button in the plug-in editor.

```pascal
FUNCTION GetPluginString(stringIndex : INTEGER) : DYNARRAY[] of CHAR;
```

```python

def vs.GetPluginString(stringIndex):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|stringIndex|INTEGER|The index of the string as represented in the plug-in editor.|

## Returns
The requested string.

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Custom


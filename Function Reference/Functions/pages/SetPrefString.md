# SetPrefString

## Description
Sets the value of the specified Vectorworks preference setting. Used with preference settings requiring a STRING value.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetPrefString(
				index : INTEGER;
				value : STRING);
```

```python

def vs.SetPrefString(index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|Preference item index.|
|value|STRING|New value for preference.|

## Remarks
Sets the value of the specified preference to the value passed.   Similar to SetPref() except it works on preferences for string values

## Examples
```pascal
SetPrefString(154,'cubits');


```

## Version
Availability: from VectorWorks9.0
## Category
* Document Settings


# SetPrefInt

## Description
Function SetPrefInt sets the value of a numeric Vectorworks preference setting.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetPrefInt(
				index : INTEGER;
				value : INTEGER);
```

```python

def vs.SetPrefInt(index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|Preference item constant.|
|value|INTEGER|New value for preference.|

## Remarks
Sets the value of the specified preference to the value passed.   Similar to SetPref() except it works on preferences for Integer values

## Examples
```pascal
SetPrefInt(17,FALSE);


```

## Version
Availability: from VectorWorks8.0
## Category
* Document Settings


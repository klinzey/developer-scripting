# SetPrefLongInt

## Description
Sets the value of the specified Vectorworks preference setting. Used with preference settings requiring a LONGINT value.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetPrefLongInt(
				index : INTEGER;
				value : LONGINT);
```

```python

def vs.SetPrefLongInt(index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|Preference item index.|
|value|LONGINT|New value for preference.|

## Remarks
Sets the value of the specified preference to the value passed.   Similar to SetPref() except it works on preferences for long integer values

## Examples
```pascal
SetPrefLongInt(55,128);


```

## Version
Availability: from VectorWorks9.0
## Category
* Document Settings


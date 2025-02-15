# GetPrefInt

## Description
Function GetPrefInt returns the value of a numeric Vectorworks preference setting.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;


```pascal
FUNCTION GetPrefInt(prefIndex : INTEGER) : INTEGER;
```

```python

def vs.GetPrefInt(prefIndex):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item constant.|

## Returns
The status of the requested preference. If the preference is a checkbox, then GetPrefInt returns TRUE or false. If it is a radio group or editable text item, then GetPrefInt returns an integer value representing that setting.

## Remarks
Returns the status of the specified preference item.  Used for preferences that return an Integer instead of a Boolean (see GetPref)

## Examples
```pascal
maxUndos:=GetPrefInt(17);


```

## Version
Availability: from VectorWorks8.0
## Category
* Document Settings


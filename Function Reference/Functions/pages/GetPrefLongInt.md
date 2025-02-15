# GetPrefLongInt

## Description
Returns the value of a Vectorworks preference setting. Used with preference settings returning a LONGINT value.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.


```pascal
FUNCTION GetPrefLongInt(prefIndex : INTEGER) : LONGINT;
```

```python

def vs.GetPrefLongInt(prefIndex):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item index.|

## Returns
Returns the value of the specified preference.<BR>
<BR>


## Remarks
Returns the status of the specified preference item.  Used for preferences that return a long integer instead of a Boolean (see GetPref)<BR>
<BR>
The status of the requested preference. If the preference is a checkbox, then GetPrefLongInt returns TRUE or false. If it is a radio group or editable text item, then GetPrefLongInt returns an integer value representing that setting.

## Examples
```pascal
convertRes2D:= GetPrefLongInt(55);


```

## Version
Availability: from VectorWorks9.0
## Category
* Document Settings


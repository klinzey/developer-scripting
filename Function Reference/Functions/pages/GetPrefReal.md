# GetPrefReal

## Description
Returns the value of a Vectorworks preference setting. Used with preference settings returning a REAL value.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;


```pascal
FUNCTION GetPrefReal(prefIndex : INTEGER) : REAL;
```

```python

def vs.GetPrefReal(prefIndex):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item index.|

## Returns
Returns the value of the specified preference.

## Remarks
Returns the status of the specified preference item.  Used for preferences that return a real instead of a Boolean (see GetPref)

## Examples
```pascal
upi:= GetPrefReal(152);


```

## Version
Availability: from VectorWorks9.0
## Category
* Document Settings


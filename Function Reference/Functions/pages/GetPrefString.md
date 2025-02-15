# GetPrefString

## Description
Returns the value of a Vectorworks preference setting. Used with preference settings returning a STRING value.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;


```pascal
FUNCTION GetPrefString(prefIndex : INTEGER) : STRING;
```

```python

def vs.GetPrefString(prefIndex):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item index.|

## Returns
Returns the value of the specified preference.

## Remarks
Returns the status of the specified preference item.  Used for preferences that return a string instead of a Boolean (see GetPref)

## Examples
```pascal
unitmark:=GetPrefString(154);


```

## Version
Availability: from VectorWorks9.0
## Category
* Document Settings


# GetPref

## Description
Function GetPref returns the on-off status of the specified preference item.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetPref(prefIndex : INTEGER) : BOOLEAN;
```

```python

def vs.GetPref(prefIndex):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|prefIndex|INTEGER|Preference item constant.|

## Examples
```pascal
SelHandleStatus:=GetPref(17);


```

## Version
Availability: from MiniCAD6.0
## Category
* Document Settings


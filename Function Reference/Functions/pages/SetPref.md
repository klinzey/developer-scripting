# SetPref

## Description
Procedure SetPref sets the on-off status of a Vectorworks preference dialog item. Parameter index specifies the preference item, and parameter status sets the on-off status of the item.&lt;BR&gt;
&lt;BR&gt;
A table of preference dialog items and their corresponding IDs may be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_f&quot;&gt;Appendix&lt;/A&gt;.


```pascal
PROCEDURE SetPref(
				index  : INTEGER;
				status : BOOLEAN);
```

```python

def vs.SetPref(index, status):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|INTEGER|Preference item constant.|
|status|BOOLEAN|On- off status of preference.|

## Examples
```pascal
SetPref(17,FALSE);


```

## Version
Availability: from MiniCAD6.0
## Category
* Document Settings


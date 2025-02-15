# SetObjectVariableLongInt

## Description
Sets the value of a Vectorworks object property. Used with properties requiring a LONGINT value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetObjectVariableLongInt(
				h     : HANDLE;
				index : INTEGER;
				value : LONGINT);
```

```python

def vs.SetObjectVariableLongInt(h, index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|
|value|LONGINT|New value for property.|

## Examples
```pascal
SetPref(17,FALSE);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


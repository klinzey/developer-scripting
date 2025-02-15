# SetObjectVariableString

## Description
Sets the value of a Vectorworks object property. Used with properties requiring a STRING value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetObjectVariableString(
				h     : HANDLE;
				index : INTEGER;
				value : DYNARRAY[] of CHAR);
```

```python

def vs.SetObjectVariableString(h, index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|
|value|DYNARRAY[] of CHAR|New value for property.|

## Examples
```pascal
SetPref(17,FALSE);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


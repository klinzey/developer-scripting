# SetObjectVariableInt

## Description
Sets the value of a Vectorworks object property. Used with properties requiring an INTEGER value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.


```pascal
PROCEDURE SetObjectVariableInt(
				h     : HANDLE;
				index : INTEGER;
				value : INTEGER);
```

```python

def vs.SetObjectVariableInt(h, index, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|
|value|INTEGER|New value for property.|

## Examples
```pascal
SetObjectVariableInt(h,1,2);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


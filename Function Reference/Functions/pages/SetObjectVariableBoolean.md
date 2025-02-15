# SetObjectVariableBoolean

## Description
Sets the ON-OFF status of a Vectorworks object property.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetObjectVariableBoolean(
				h      : HANDLE;
				index  : INTEGER;
				status : BOOLEAN);
```

```python

def vs.SetObjectVariableBoolean(h, index, status):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|
|status|BOOLEAN|New status for property.|

## Examples
```pascal
SetObjectVariableBoolean(17,FALSE);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


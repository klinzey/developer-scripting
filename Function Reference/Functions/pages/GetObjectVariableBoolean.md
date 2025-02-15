# GetObjectVariableBoolean

## Description
Returns the ON-OFF status of a Vectorworks object property. &lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.


```pascal
FUNCTION GetObjectVariableBoolean(
				h     : HANDLE;
				index : INTEGER) : BOOLEAN;
```

```python

def vs.GetObjectVariableBoolean(h, index):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|

## Returns
Returns a BOOLEAN value indicating the ON-OFF status of the property.

## Examples
```pascal
castShadow:= GetObjectVariableBoolean(h,53);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


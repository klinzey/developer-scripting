# GetObjectVariableString

## Description
Returns the value of a Vectorworks object property. Used with properties returning a STRING value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetObjectVariableString(
				h     : HANDLE;
				index : INTEGER) : DYNARRAY[] of CHAR;
```

```python

def vs.GetObjectVariableString(h, index):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|

## Returns
Returns the value of the property as a STRING value.

## Examples
```pascal
dimstdName:= GetObjectVariableString(h,27);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


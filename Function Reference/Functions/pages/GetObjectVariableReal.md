# GetObjectVariableReal

## Description
Returns the value of a Vectorworks object property. Used with properties returning a REAL value. Always returns values in mm, regardless of document units.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetObjectVariableReal(
				h     : HANDLE;
				index : INTEGER) : REAL;
```

```python

def vs.GetObjectVariableReal(h, index):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|

## Returns
Returns the value of the property as a REAL value.

## Examples
```pascal
dim_offset:= GetObjectVariableReal(h,4);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


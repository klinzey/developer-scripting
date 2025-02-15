# GetObjectVariableLongInt

## Description
Returns the value of a Vectorworks object property. Used with properties returning a LONGINT value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetObjectVariableLongInt(
				h     : HANDLE;
				index : INTEGER) : LONGINT;
```

```python

def vs.GetObjectVariableLongInt(h, index):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|

## Returns
Returns the value of the property as a LONGINT value.

## Examples
```pascal
p:= GetObjectVariableLongInt(h,579);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


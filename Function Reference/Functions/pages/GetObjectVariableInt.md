# GetObjectVariableInt

## Description
Returns the value of a Vectorworks object property. Used with properties returning an INTEGER value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the &lt;A HREF=&quot;../Appendix/appendix.html#appx_g&quot;&gt;Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetObjectVariableInt(
				h     : HANDLE;
				index : INTEGER) : INTEGER;
```

```python

def vs.GetObjectVariableInt(h, index):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|

## Returns
Returns the value of the property as an INTEGER value.

## Examples
```pascal
numCavities:= GetObjectVariableInt(h,199);


```

## Version
Availability: from VectorWorks9.0
## Category
* Object Info


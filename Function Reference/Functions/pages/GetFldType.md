# GetFldType

## Description
Returns a constant indicating the data type of a specified field in the referenced record.&lt;BR&gt;
&lt;BR&gt;
Please refer to the &lt;A HREF=&quot;../Appendix/appendix.html#fieldtype&quot;&gt;VectorScript Appendix&lt;/A&gt; for specific field data types and formatting.
&lt;BR&gt;
&lt;BR&gt;
For Plug-in Object Parameter Records, the field types are documented in the &lt;A HREF=&quot;../Appendix/appendix.html#paramtype&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;


```pascal
FUNCTION GetFldType(
				h : HANDLE;
				t : INTEGER) : INTEGER;
```

```python

def vs.GetFldType(h, t):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to record.|
|t|INTEGER|Field index (range of 1 - n).|

## Remarks
Returns a constant indicating which type of field is specified by the field number &quot;t&quot; of record &quot;h&quot;.  The field type constants are listed in an appendix in the vectorscript manual.<BR>
<BR>
[sd 8/14/98]

## Examples
```pascal
fieldType:=GetFldType(recordHandle,3);
```

## Version
Availability: from MiniCAD
## Category
* Database / Record


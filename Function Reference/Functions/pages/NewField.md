# NewField

## Description
Creates a new field in a specified record format. If the record does not exist, a new one is created using the specified record name.&lt;BR&gt;
&lt;BR&gt;
Please refer to the &lt;A HREF=&quot;../Appendix/appendix.html#fieldtype&quot;&gt;VectorScript Appendix&lt;/A&gt; for specific field data types and formatting.
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE NewField(
				recName    : DYNARRAY[] of CHAR;
				fieldName  : DYNARRAY[] of CHAR;
				fieldValue : DYNARRAY[] of CHAR;
				fType      : INTEGER;
				fFlag      : INTEGER);
```

```python

def vs.NewField(recName, fieldName, fieldValue, fType, fFlag):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|recName|DYNARRAY[] of CHAR|Name of record to which field will be added. |
|fieldName|DYNARRAY[] of CHAR|Name of new field.|
|fieldValue|DYNARRAY[] of CHAR|Default value for new field.|
|fType|INTEGER|Data type of new field.|
|fFlag|INTEGER|Display style of field.|

## Examples
```pascal
NewField('Part Info','Serial No.','A-0000',4,0);


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


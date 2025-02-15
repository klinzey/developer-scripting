# SetRField

## Description
Assigns a new value to an existing field of a record attached to the referenced object.

```pascal
PROCEDURE SetRField(
				h      : HANDLE;
				record : DYNARRAY[] of CHAR;
				field  : DYNARRAY[] of CHAR;
				value  : DYNARRAY[] of CHAR);
```

```python

def vs.SetRField(h, record, field, value):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to a object with an attached record.|
|record|DYNARRAY[] of CHAR|Name of record to be updated.|
|field|DYNARRAY[] of CHAR|Name of field to be updated.|
|value|DYNARRAY[] of CHAR|New value for field.|

## Remarks
Update the RecordNode attached to object &quot;h&quot; by setting the field &quot;field&quot; of record format named &quot;record&quot; to the value &quot;value&quot;.  The object &quot;h&quot; is redrawn afterward to support the symbol &quot;link text to record&quot; feature.<BR>
<BR>
Replaces obsolete function &quot;Field&quot;.<BR>


## Examples
```pascal
SetRField(HandleToObject,'Part Info','Serial No.','P-4322');


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


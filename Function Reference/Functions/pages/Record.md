# Record

## Description
Replaces an existing record with a new version of the same record. Parameter s specifies the record to be updated.

```pascal
PROCEDURE Record(
				h : HANDLE;
				s : DYNARRAY[] of CHAR);
```

```python

def vs.Record(h, s):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|s|DYNARRAY[] of CHAR|Name of record to be updated.|

## Remarks
Delete any existing record named &quot;s&quot; on &quot;h&quot;, Create new record for format named &quot;s&quot;, attach to &quot;h&quot;.<BR>
<BR>
[sd 8/14/98]

## Examples
```pascal
Record(handleToObj,'Vendor Information');
```

## Version
Availability: from MiniCAD
## Category
* Database / Record


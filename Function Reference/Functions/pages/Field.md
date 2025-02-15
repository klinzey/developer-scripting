# Field

## Description
Obsolete.  &lt;BR&gt;


```pascal
PROCEDURE Field(
				h  : HANDLE;
				s1 : STRING;
				s2 : STRING;
				s3 : STRING);
```

```python

def vs.Field(h, s1, s2, s3):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE||
|s1|STRING||
|s2|STRING||
|s3|STRING||

## Remarks
Obsolete function maintained for compatibility with old scripts. Use &quot;SetRField&quot; for new scripts.  See &quot;SetRField&quot;.<BR>
<BR>
Update the RecordNode attached to object &quot;h&quot; by setting the field &quot;s2&quot; of format &quot;s1&quot; to the value &quot;s3&quot;.  The object is not redrawn immediately, so don't call this for a symbol which uses the &quot;link text to record&quot; feature.<BR>
<BR>
[sd 9/14/98]

## See Also
VS Functions:
[SetRField](SetRField.md)

## Version
Availability: from MiniCAD
## Category
* Database / Record


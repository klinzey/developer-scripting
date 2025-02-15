# Trunc

## Description
Truncates the decimal portion of the specified REAL number, returning the result as a LONGINT value.&lt;BR&gt;
&lt;BR&gt;
Note that direct assignment of a REAL to a LONGINT will result in rounding the REAL to the &amp;lt;i&amp;gt;nearest&amp;lt;/i&amp;gt; LONGINT, whereas Trunc always &amp;quot;rounds down&amp;quot; (if the number is positive).&lt;BR&gt;


```pascal
FUNCTION Trunc(v : REAL) : LONGINT;
```

```python

def vs.Trunc(v):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|v|REAL|Real value to truncate.|

## Version
Availability: from MiniCAD
## Category
* Math - General


# GetParametricRecord

## Description
Returns the handle to the parametric record attached the referenced object.&lt;BR&gt;
&lt;BR&gt;
Parametric record is a hidden record format containing the parameter values of the parametric object.&lt;BR&gt;
Only parametric objects have parametric records.

```pascal
FUNCTION GetParametricRecord(h : HANDLE) : HANDLE;
```

```python

def vs.GetParametricRecord(h):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to a parametric object|

## Returns
Returns a handle to the record, or NIL if the record doesn't exist (e.g. not a parametric object passed)

## Version
Availability: from Vectorworks 2011
## Category
* Database / Record


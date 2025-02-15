# NumRecords

## Description
Returns the number of records attached to the referenced object. &lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION NumRecords(h : HANDLE) : INTEGER;
```

```python

def vs.NumRecords(h):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
numAttached:=NumRecords(HandleToObject);


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


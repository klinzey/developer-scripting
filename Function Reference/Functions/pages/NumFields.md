# NumFields

## Description
Returns the number of fields in the referenced record.&lt;BR&gt;


```pascal
FUNCTION NumFields(h : HANDLE) : INTEGER;
```

```python

def vs.NumFields(h):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to record.|

## Examples
```pascal
totalFields:=NumFields(HandleToRecord);


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


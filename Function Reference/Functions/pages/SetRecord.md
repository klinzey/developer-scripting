# SetRecord

## Description
Assigns an instance of an existing record format to the referenced object . &lt;BR&gt;


```pascal
PROCEDURE SetRecord(
				h      : HANDLE;
				record : DYNARRAY[] of CHAR);
```

```python

def vs.SetRecord(h, record):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|record|DYNARRAY[] of CHAR|Name of record to assign to object.|

## Examples
```pascal
SetRecord(HandleToObject,'Part Info');


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


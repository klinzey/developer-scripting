# GetFldName

## Description
Returns the name of the specified field in the referenced record.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetFldName(
				h     : HANDLE;
				index : INTEGER) : STRING;
```

```python

def vs.GetFldName(h, index):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to record.|
|index|INTEGER|Number of field whose name will be returned (in a range of 1-n).|

## Examples
```pascal
FName:=GetFldName(HandleToRecord,1);


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


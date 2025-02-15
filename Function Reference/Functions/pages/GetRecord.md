# GetRecord

## Description
Returns the handle to a specified record attached the referenced object.

```pascal
FUNCTION GetRecord(
				h   : HANDLE;
				cnt : INTEGER) : HANDLE;
```

```python

def vs.GetRecord(h, cnt):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|cnt|INTEGER|Index of attached record (in a range of 1 -  n).|

## Examples
```pascal
handleToRecord := GetRecord(handleToObject,3);


```

## Version
Availability: from MiniCAD
## Category
* Database / Record


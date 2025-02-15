# GetPartDataID

## Description
Return the numeric value assigned to this part instance represented by the specified sub-object.&lt;BR&gt;
The sub-object must be an object that was tagged as a part.

```pascal
FUNCTION GetPartDataID(objectHandle : HANDLE) : LONGINT;
```

```python

def vs.GetPartDataID(objectHandle):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|The sub-object handle.|

## Returns
The numeric value assigned to this part instance.

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom


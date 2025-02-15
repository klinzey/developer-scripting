# GetPartInstanceName

## Description
Return the unique name assigned to this part instance represented by the specified sub-object.&lt;BR&gt;
The sub-object must be an object that was tagged as a part.

```pascal
FUNCTION GetPartInstanceName(objectHandle : HANDLE) : STRING;
```

```python

def vs.GetPartInstanceName(objectHandle):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|The sub-object handle.|

## Returns
The unique name assigned to this part instance.

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom


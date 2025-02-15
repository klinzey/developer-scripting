# SetObjectTags

## Description
Lets the user set a list of Tags on an object such as a Class,Layer or Resource.

```pascal
FUNCTION SetObjectTags(
				objectHandle : HANDLE;
				arrTags      : ARRAY) : BOOLEAN;
```

```python

def vs.SetObjectTags(objectHandle, arrTags):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|The object to set Tags on.|
|arrTags|ARRAY|The arra of Tag Strings.|

## Version
Availability: from Vectorworks 2019
## Category
* General Edit


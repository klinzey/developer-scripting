# GetObjectTags

## Description
Lets the user query the list of Tags set on an object such as a Class,Layer or Resource.

```pascal
FUNCTION GetObjectTags(
				objHandle      : HANDLE;
				VAR outArrTags : ARRAY) : BOOLEAN;
```

```python

def vs.GetObjectTags(objHandle):
    return (BOOLEAN, outArrTags)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objHandle|HANDLE|The handle to the object to query Tags from.|
|outArrTags|ARRAY|The output array of Tags queried from the object.|

## Version
Availability: from Vectorworks 2019
## Category
* General Edit


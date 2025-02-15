# CreateDuplicateObject

## Description
Duplicates the specified object and inserts the new  object into the container.  If container is nil, the new object will be inserted in the active container.

```pascal
FUNCTION CreateDuplicateObject(
				objectToDuplicate : HANDLE;
				containerHandle   : HANDLE) : HANDLE;
```

```python

def vs.CreateDuplicateObject(objectToDuplicate, containerHandle):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectToDuplicate|HANDLE|The object to be duplicated|
|containerHandle|HANDLE|The container to the newly duplicated object|

## Remarks
This should be used inplace of a SetParent.

## Version
Availability: from VectorWorks12.5
## Category
* Object Editing


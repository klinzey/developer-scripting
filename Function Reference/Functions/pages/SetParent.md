# SetParent

## Description
Removes the object from its current container and places it within the given container. For example, SetParent can be used to put the referenced object into a group, or into a symbol definition, or to change the layer of the referenced object.

```pascal
FUNCTION SetParent(
				obj       : HANDLE;
				container : HANDLE) : BOOLEAN;
```

```python

def vs.SetParent(obj, container):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to the object to move.|
|container|HANDLE|Handle to the object that will become the parent of the obj variable.|

## Remarks
This function will fail if obj is being moved from a non-regenerable list of a plug-in to a regenrable list of a plug-in

## Examples
```pascal
PROCEDURE SetParentExample;

VAR

	h1, h2 :HANDLE;

	boo :BOOLEAN;

BEGIN

	h1 := FSActLayer;

	h2 := NextObj(h1);

	boo := SetParent(h2, h1);

END;

RUN(SetParentExample);
```

## See Also
VS Functions:
[CreateDuplicateObject](CreateDuplicateObject.md)

## Version
Availability: from VectorWorks10.0
## Category
* Document List Handling


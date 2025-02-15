# RemoveSubMtrlFromMtl

## Description
Removes a Simple material from a Compound material.

```pascal
FUNCTION RemoveSubMtrlFromMtl(
				hMaterial   : HANDLE;
				subMtrlName : STRING) : Boolean;
```

```python

def vs.RemoveSubMtrlFromMtl(hMaterial, subMtrlName):
    return Boolean
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hMaterial|HANDLE|Handle of a Compound material|
|subMtrlName|STRING|Name of a Simple material to be deleted|

## Returns
Returns true if successful; false otherwise. Returns false if the simple material is not found.

## Version
Availability: from Vectorworks 2021
## Category
* Object Attributes


# AddSubMtrlToMtrl

## Description
Adds a Simple material to a Compound material. Sets the fraction of the Simple material as a relation to the whole. Fraction can have value between 0.0 and 1.0. &amp;quot;Primary&amp;quot; material is a simple material which carries the graphical attributes to be used by the compound material.

```pascal
FUNCTION AddSubMtrlToMtrl(
				hMaterial   : HANDLE;
				subMtrlName : STRING;
				fraction    : REAL;
				makePrimary : BOOLEAN) : Boolean;
```

```python

def vs.AddSubMtrlToMtrl(hMaterial, subMtrlName, fraction, makePrimary):
    return Boolean
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hMaterial|HANDLE|Handle of a Compound material|
|subMtrlName|STRING|Name of a Simple material to be added|
|fraction|REAL|Fraction of the Simple material|
|makePrimary|BOOLEAN|True if this Simple material should become the primary material of the Compound material|

## Returns
Returns true if successful; false otherwise. Function fails if the simple material already was added.

## Version
Availability: from Vectorworks 2021
## Category
* Object Attributes


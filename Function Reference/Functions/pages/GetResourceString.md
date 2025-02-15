# GetResourceString

## Description
Returns the specified resource string from a resource file.

```pascal
PROCEDURE GetResourceString(
				VAR theString : DYNARRAY[] of CHAR;
				id            : INTEGER;
				index         : INTEGER);
```

```python

def vs.GetResourceString(id, index):
    return theString
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theString|DYNARRAY[] of CHAR|The string contained within the resource.|
|id|INTEGER|The ID of the resource.|
|index|INTEGER|The index of the string resource.|

## See Also
VS Functions:
[SetVSResourceFile](SetVSResourceFile.md)

## Version
Availability: from VectorWorks9.0
## Category
* Strings


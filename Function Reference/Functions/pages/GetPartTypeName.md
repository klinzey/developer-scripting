# GetPartTypeName

## Description
Return the part type for the specified sub-object.&lt;BR&gt;
The sub-object must be an object that was tagged as a part.

```pascal
FUNCTION GetPartTypeName(objectHandle : HANDLE) : STRING;
```

```python

def vs.GetPartTypeName(objectHandle):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHandle|HANDLE|The sub-object handle.|

## Returns
The part type name for the specified sub-object. The sub-object must be an object that was tagged as a part.

## See Also
VS Functions:
[TagSubObjectAsPart](TagSubObjectAsPart.md)

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom


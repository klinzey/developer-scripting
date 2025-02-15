# GetActualNameFromResourceList

## Description
Returns the actual name of the indicated item in the specified resource list. This call will delete the filename that is appended for resources with same name from different files.&lt;BR&gt;


```pascal
FUNCTION GetActualNameFromResourceList(
				listID : LONGINT;
				index  : LONGINT) : DYNARRAY[] of CHAR;
```

```python

def vs.GetActualNameFromResourceList(listID, index):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|listID|LONGINT|an ID for a resouce list created by the BuildResourceList function.|
|index|LONGINT|an index into the list.|

## Remarks
To get the display name use GetNameFromResourceList.

## Examples
```pascal
displayName := GetActualNameFromResourceList(listID, index);
```

## See Also
VS Functions:
[GetNameFromResourceList](GetNameFromResourceList.md)

## Version
Availability: from VectorWorks12.0
## Category
* Document List Handling


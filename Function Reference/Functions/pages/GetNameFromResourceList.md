# GetNameFromResourceList

## Description
Returns the name to display of the indicated item in the specified resource list.  If the list has items with the same name from different files, the display name will have the filename added to it in parentheses.

```pascal
FUNCTION GetNameFromResourceList(
				listID : LONGINT;
				index  : LONGINT) : DYNARRAY[] of CHAR;
```

```python

def vs.GetNameFromResourceList(listID, index):
    return DYNARRAY[] of CHAR
```

## Parameters
|Name|Type|Description|
|---|---|---|
|listID|LONGINT|an ID for a resouce list created by the BuildResourceList function.|
|index|LONGINT|an index into the list.|

## Remarks
To get the actual name use GetActualNameFromResourceList.

## Examples
```pascal
hatchName := GetNameFromResourceList(listID, index);

if (pos('P', hatchName) = 1) then

	DeleteResourceFromList(listID, index)


```

## See Also
VS Functions:
[GetActualNameFromResourceList](GetActualNameFromResourceList.md)

## Version
Availability: from VectorWorks12.0
## Category
* Document List Handling


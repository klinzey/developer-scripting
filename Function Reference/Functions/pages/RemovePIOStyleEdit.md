# RemovePIOStyleEdit

## Description
Removes an item from the edit style mapping list.

```pascal
FUNCTION RemovePIOStyleEdit(
				hObj    : HANDLE;
				keyName : STRING) : BOOLEAN;
```

```python

def vs.RemovePIOStyleEdit(hObj, keyName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObj|HANDLE|Handle to a plug-in object or plug-in style|
|keyName|STRING|Name of item to remove from list.|

## Returns
TRUE if item is removed from list.<BR>
<BR>
FALSE if hObj is NULL; if hObj is not a styled plug-in object or plug-in style<BR>
FALSE if item does not appear in list.

## See Also
VS Functions:
[AddToPIOStyleEdit](AddToPIOStyleEdit.md)

## Version
Availability: from Vectorworks 2018
## Category
* Objects - Custom


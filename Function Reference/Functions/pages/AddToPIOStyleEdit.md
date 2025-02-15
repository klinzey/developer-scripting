# AddToPIOStyleEdit

## Description
Adds an item to a plug-in style's default edit list. This is only used by objects that use the default edit style dialog.&lt;BR&gt;
&lt;BR&gt;
By default, only those parameters shown in the object info palette will be listed in the edit style mapping dialg. Pass the following values to add or remove an item this list.&lt;BR&gt;
&lt;BR&gt;
Values:&lt;BR&gt;
1 - Add to the edit style map dialog.&lt;BR&gt;
2 - Remove from the edit stkyle map dialog.&lt;BR&gt;
&lt;BR&gt;
&lt;BR&gt;
To remove an entry from this list use RemovePIOStyleEdit.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION AddToPIOStyleEdit(
				hObj        : HANDLE;
				keyName     : STRING;
				editType    : INTEGER;
				displayName : STRING) : BOOLEAN;
```

```python

def vs.AddToPIOStyleEdit(hObj, keyName, editType, displayName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObj|HANDLE|Handle to a plug-in object or plug-in object style|
|keyName|STRING|Universal name of parameter or iother item to add to the edit style map list|
|editType|INTEGER|1 - Add to edit list 2 - Remove from edit list|
|displayName|STRING|The display name to use in the style map dialog. If an empy string is passed the keyName will be used.|

## Returns
TRUE if key is added to the list.<BR>
<BR>
FALSE if hObj is NULL; if hObj is not a styled plug-in object or plug-in style<BR>
FALSE if item already appear in list. Use RemoveFromPluginStyleEditList first.

## See Also
VS Functions:
[RemovePIOStyleEdit](RemovePIOStyleEdit.md)

## Version
Availability: from Vectorworks 2018
## Category
* Objects - Custom


# SetWallInsLocByStyle

## Description
Sets whether the wall insert location of a symbol definition, plug-in object style, or plug-in object is by style.

```pascal
FUNCTION SetWallInsLocByStyle(
				hObject : HANDLE;
				byStyle : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetWallInsLocByStyle(hObject, byStyle):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE|The symbol definition, plug-in object style, or plug-in object.|
|byStyle|BOOLEAN|Whether the wall insert location is by style.|

## Returns
Whether the call succeeded.

## See Also
VS Functions:
[GetWallInsLocByStyle](GetWallInsLocByStyle.md)

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom


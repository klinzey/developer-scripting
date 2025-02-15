# SetUseWllClsrByStyle

## Description
Sets whether the use wall closure setting of a symbol definition, plug-in object style, or plug-in object is by style.

```pascal
FUNCTION SetUseWllClsrByStyle(
				hObject : HANDLE;
				byStyle : BOOLEAN) : BOOLEAN;
```

```python

def vs.SetUseWllClsrByStyle(hObject, byStyle):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hObject|HANDLE|The symbol definition, plug-in object style, or plug-in object.|
|byStyle|BOOLEAN|Whether the use wall closure setting is by style.|

## Returns
Whether the call succeeded.

## See Also
VS Functions:
[GetUseWllClsrByStyle](GetUseWllClsrByStyle.md)

## Version
Availability: from Vectorworks 2022
## Category
* Objects - Custom

